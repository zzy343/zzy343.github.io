import streamlit as st
import random
import time
import math

class HeartAnimationWeb:
    def __init__(self):
        # 网页配置：标题、图标
        st.set_page_config(page_title="爱心关心提示", page_icon="❤️")
        st.title("❤️ 爱心关心提示动画")
        
        # 保留原逻辑：文字、颜色、爱心参数
        self.tips = [
            '金龙', '招叶', '公牛', '旭泰',
            '旭泰记得喝水', '旭泰按时吃饭', '旭泰别熬夜了', '旭泰照顾好自己',
            '旭泰注意身体', '旭泰记得运动', '旭泰放松一下', '旭泰保持微笑',
            '旭泰劳逸结合', '旭泰别太劳累', '旭泰记得午休', '旭泰多吃水果',
            '旭泰出去走走', '旭泰呼吸新鲜空气', '旭泰保持好心情', '旭泰别久坐',
            '旭泰记得早餐', '旭泰保护眼睛', '旭泰注意保暖', '旭泰别着凉',
            '旭泰保持健康', '旭泰平安喜乐', '旭泰开心每一天', '旭泰一切顺利',
            '旭泰万事如意', '旭泰心想事成'
        ]
        
        self.bg_colors = [
            'lightpink', 'skyblue', 'lightgreen', 'lavender', 'lightyellow',
            'plum', 'coral', 'bisque', 'aquamarine', 'mistyrose'
        ]
        
        # 适配网页的爱心参数
        self.window_count = 100  # 爱心由100个“小卡片”组成
        self.scale = 45  # 控制爱心整体大小
        self.heart_points = self.generate_heart_points()  # 计算爱心坐标
        self.empty_containers = []  # 存储网页占位组件

    def heart_shape(self, t):
        # 原爱心数学公式（保留）
        x = 16 * (math.sin(t) ** 3)
        y = -(13 * math.cos(t) - 5 * math.cos(2*t) - 2 * math.cos(3*t) - math.cos(4*t))
        return x * self.scale, y * self.scale

    def generate_heart_points(self):
        # 计算爱心在网页中的坐标（适配Streamlit布局）
        points = []
        # 网页中心坐标（Streamlit主区域宽度约800px，高度自适应）
        center_x, center_y = 400, 300
        for i in range(self.window_count):
            t = 2 * math.pi * i / self.window_count
            x, y = self.heart_shape(t)
            # 计算每个“小卡片”的坐标（确保爱心居中且位置适配）
            card_x = center_x + x - 70  # 减去卡片宽度的一半（140/2）
            card_y = center_y + y - 22  # 减去卡片高度的一半（45/2）
            points.append((card_x, card_y))
        return points

    def create_web_card(self, x, y):
        # 在网页中创建“小卡片”（替代tkinter窗口）
        empty = st.empty()
        self.empty_containers.append(empty)
        
        # 随机选择文字和背景色
        tip = random.choice(self.tips)
        bg = random.choice(self.bg_colors)
        
        # 用HTML/CSS模拟卡片样式（Streamlit支持直接渲染HTML）
        card_html = f"""
        <div style="
            position: absolute;
            left: {x}px;
            top: {y}px;
            width: 140px;
            height: 45px;
            background-color: {bg};
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: '仿宋', serif;
            font-size: 12px;
            font-weight: bold;
            color: #333;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        ">
            {tip}
        </div>
        """
        # 渲染卡片到网页
        empty.markdown(card_html, unsafe_allow_html=True)

    def start_web_animation(self):
        # 网页端动画主逻辑
        st.info("💖 准备开始绘制爱心...点击下方按钮启动！")
        # 添加启动按钮（增强交互）
        if st.button("启动爱心动画"):
            # 1. 逐步显示爱心卡片
            st.success("💖 正在绘制大爱心...")
            for x, y in self.heart_points:
                self.create_web_card(x, y)
                time.sleep(0.2)  # 控制显示速度
            
            # 2. 停留3秒
            st.success("💕 大爱心完成！将在3秒后关闭...")
            time.sleep(3)
            
            # 3. 逐步关闭卡片
            st.success("✨ 正在关闭窗口...")
            for container in reversed(self.empty_containers):
                container.empty()  # 清空占位符（删除卡片）
                time.sleep(0.1)
            
            st.success("✅ 动画结束！可再次点击按钮重新播放～")

# 主函数（启动网页应用）
def main():
    app = HeartAnimationWeb()
    app.start_web_animation()

if __name__ == "__main__":
    main()
