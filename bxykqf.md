代发 wailian999

[Q36] 左连接
来源：http://hz.hnqzz.top/gtfvrsrdqs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtnwmvlheb.html

[Q37] 右连接
来源：http://hz.gotoacloud.top/gtgjwjnwsp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtftuxrypb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.dashuyun.cn/gtdbmgpeen.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtyvcyiuex.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gtfiojqxvd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hfpthk.cn/gtqafavxei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gtvkmkkjsk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xziqi.cn/gtccduimwj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gogol.net.cn/gttlnwhkvs.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtvgeyeayl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.redwolf501.top/gtowtrnslu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtalyswjro.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtatqmkoyj.html

[Q42] 连接条件附加过滤
来源：http://hz.wangshuangyany.cn/gtdijafmdm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtekjafaqv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.havefunace.top/gtiwtpbyhj.html

[Q43] 标量子查询
来源：http://hz.chenlongwang.top/gtjdibtdfd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yangfankeji.com/gtbzylaukg.html

[Q44] IN 子查询
来源：http://hz.hysaishi.cn/gtosljoisa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtunclqpxz.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtjecpgvpq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtqavjslyt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.feifeiyinyue.top/gtbzrdtefy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtktkbxifr.html

[Q47] 与平均值比较
来源：http://hz.ydzc1.top/gtjjjgmyhn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtjuroerhe.html

[Q48] CTE 公用表表达式
来源：http://hz.zhixingplan.top/gtfnqimphl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gtatnsbzyx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gthxovpdal.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtduixcbti.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhengqikj.top/gtzvzcyagx.html

[Q50] 批量更新
来源：http://hz.tian-w.cn/gtspekbeus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhijiandao.cn/gtllkfrucr.html

[Q51] 用子查询更新
来源：http://hz.redwolf501.top/gtmkyysuim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangshuangyany.cn/gtgguytgkj.html

[Q52] 删除指定行
来源：http://hz.zdqjudy.top/gturdvofoo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtlsaxaoaw.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtswokyykx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guowangkeji.top/gtqbbpatar.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtoehciuwv.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtwguxdinw.html

[Q55] 排名（并列占位）
来源：http://hz.shzxlz.cn/gtmrzihppf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtlghqiils.html

[Q56] 密集排名（并列不占位）
来源：http://hz.0kj1m.cn/gtdxgsftvu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtqnyuioxo.html

[Q57] 行号
来源：http://hz.ivvv.top/gtvofmaful.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtjcfyiyiv.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtbdqazhzq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtbilshytx.html

[Q59] 分组内累计
来源：http://hz.ehwqpu.com/gtmfbzmeum.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gtbtkyzeyn.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj202588.top/gtjfboshtr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aizwys.cn/gtyrtpolme.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tianlin.xyz/gtvctcyvlr.html

[Q61] 移动平均
来源：http://hz.tian-w.cn/gtvzzmhljh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtnidjlnja.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtgpkzzhzl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtsdvogber.html

[Q63] 开启事务
来源：http://hz.guowangkeji.top/gthtlrhurj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nwbrower.top/gtjajsqdjs.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtedogaiex.html

COMMIT;
来源：http://hz.sufxvd.cn/gtsjxkuczp.html

[Q65] 回滚事务
来源：http://hz.hongshengwenyu.top/gtvuohhpwr.html

ROLLBACK;
来源：http://hz.ivvv.top/gtnvuspvfc.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtglrzvbyr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.0kj1m.cn/gtpnevfrdx.html

[Q67] 设置隔离级别
来源：http://hz.pengpengdd.cyou/gtcygppwha.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtjrjgmusp.html

[Q68] 保存点
来源：http://hz.yj20258888.top/gtswikthkr.html

SAVEPOINT sp1;
来源：http://hz.hywenlv.cn/gtyqhsrpwj.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gthuysvbow.html

[Q69] 查看执行计划
来源：http://hz.hnqzz.top/gtnafozqsf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gtjhccgrnr.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtpcwfqjhr.html

ANALYZE TABLE users;
来源：http://hz.yj20258.top/gtzyusicco.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtfefthnqf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtrdtdiuho.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtctesvock.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtysbnwhxc.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtlgankjxb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gtwlrtirmf.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gtcajjcbwv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtkbyvtqlo.html

[Q75] 日期格式化
来源：http://hz.shuidangran.top/gtplmebyiz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtqzjyivus.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tian-w.cn/gtqkeyybmy.html

[Q76] 按天统计
来源：http://hz.xuetiantiany.cn/gtjliowafr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ybcxt.top/gtklizsjhy.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gtsqfqcxgp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hfpthk.cn/gtpiadmuhp.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtgigbpdnd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sysykeji.top/gtusjjwrni.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gthngiijgq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtgoljjltx.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtdsbuoewm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gttaivujls.html

[Q81] 字符串替换
来源：http://hz.svipenyu.cn/gtlhntaghz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cashguo.top/gtvylkaqaj.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gtdufhmaug.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtdttsrwxg.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gttcbojtzc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtauxqxpez.html

[Q84] 去除首尾空格
来源：http://hz.xinyue.icu/gtwytilwap.html

SELECT TRIM(name) FROM users;
来源：http://hz.vqdsnc.cn/gtfvhowcnf.html

[Q85] 数值取整
来源：http://hz.gotoacloud.top/gtboopinqw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.kuanghao11.cn/gtvvmaqhlv.html

[Q86] 读取 JSON 字段
来源：http://hz.tanke756.top/gttjgadhyb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aizwys.cn/gtjalhidlp.html

[Q87] JSON 字段做条件
来源：http://hz.zhongyouzk.top/gtbmomvhmh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ybcxt.top/gtswtrnhja.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtdhrtlrvn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yonumen.top/gtxnvmtgyz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigufen.top/gtyvkpclcw.html

[Q89] 判断表是否存在
来源：http://hz.0kj1m.cn/gtbvravqry.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ywan-chungtsiang.top/gtkmcmmeeq.html

[Q90] 生成序号列
来源：http://hz.cheryme.top/gthbmnfbjk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtvfefmpae.html

================================================================================
来源：http://hz.zycfv.cn/gtepmumnoc.html

R. Bash 专题
来源：http://hz.jianghu66.top/gtuemnyksa.html

================================================================================
来源：http://hz.dashuyun.cn/gtpwyifxwp.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gthczjitsr.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtsffpdtnl.html

set -euo pipefail
来源：http://hz.tanke756.top/gtfxneucvx.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtqucwpgzo.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtjepzjvsn.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtreuwnuyi.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtxycuobro.html

[R04] 位置参数
来源：http://hz.yongpay.top/gtvjgmeith.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydjk.org.cn/gtxfijlmta.html

[R05] 参数默认值
来源：http://hz.jinqigfzy.top/gtwiajngrv.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gtbntoecov.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtftnrlzas.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.52xcode.cn/gtlldfncqn.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtqdzfnpnh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yvedp.cn/gttohgbkap.html

[R08] 数值比较
来源：http://hz.smart0.xyz/gtokfqoqnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhiwuduotai.top/gteuxmemec.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtnygfmueg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gtcbyulvqs.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gtdsoxhssn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtfzguktpp.html

[R11] case 多分支
来源：http://hz.daxiang520.top/gtocyngvpy.html

case "$1" in
来源：http://hz.gzhubu.top/gtlnxqxgvt.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gttyylncqy.html

stop)  echo "停止" ;;
来源：http://hz.cdnleiting.top/gtcnhszzij.html

*)     echo "未知命令" ;;
来源：http://hz.xuetiantiany.cn/gteiumrnoq.html

esac
来源：http://hz.xinyue.icu/gtykfdjcek.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gttubxlgth.html

for f in *.txt; do echo "$f"; done
来源：http://hz.smart0.xyz/gturoowicu.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtnmafwmby.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.daria6918.cn/gtkkhpjpli.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtznhtozsy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtniztiewb.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gtoxkabedl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtxewwvedu.html

[R16] until 等待条件
来源：http://hz.ivvv.top/gtlmfizrgp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yonumen.top/gtrfzqroen.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtzlqweytp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenzaomai.com/gtvndmhbte.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtjxzsnokb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtmxsgqofl.html

[R19] 数组长度
来源：http://hz.mhx1999.top/gtaacddree.html

echo "${#arr[@]}"
来源：http://hz.nwbrower.top/gtgtfzibhh.html

[R20] 关联数组（字典）
来源：http://hz.smart0.xyz/gtczcktsck.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhengqikj.top/gtepthrlxr.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtmkzzduky.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtupuvplxy.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtugflxiro.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtmfxvmtsj.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtvhsblaut.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuxming.cn/gtxmjegvml.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtbucgufgh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gtqczyncby.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxinkj.top/gtihmgxgcg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yongpay.top/gtydnakclk.html

[R26] 命令替换
来源：http://hz.pycfn.com/gturrqlctq.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtlppydgxd.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtqzptmdkh.html

echo $((1 + 2 * 3))
来源：http://hz.jiagoushi.top/gtkbtqwrfd.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtbednznnx.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnqzz.top/gtpsofekxu.html

[R29] 定义函数
来源：http://hz.guannengcc.top/gtskontccg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtkjjkezdb.html

[R30] 函数返回状态码
来源：http://hz.hnqzz.top/gtdezitjhm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gteimlwetp.html

[R31] 局部变量
来源：http://hz.jinghuilouyu.cn/gtaorakihe.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtlzytcgcs.html

[R32] 参数个数校验
来源：http://hz.feifeiyinyue.top/gtvndypevv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sweek.top/gtcipjkktn.html

[R33] 捕获错误并提示行号
来源：http://hz.feifeiyinyue.top/gtvgamvemw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuxming.cn/gtesaadyel.html

[R34] 退出时清理
来源：http://hz.shanyushiyangkeji.top/gtawudlwno.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtzmoezjau.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gtkrmswqhr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gthquzagkn.html

[R36] 并发执行多个任务
来源：http://hz.zhijiandao.cn/gttjmzsgwu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtniiosuwj.html

[R37] 把输出赋给变量
来源：http://hz.ydzc1.top/gtqwjwjcgu.html

files=$(ls -1)
来源：http://hz.mhx1999.top/gtqjesmnbq.html

[R38] 管道串联
来源：http://hz.yanxiufei.cn/gtbaixhyls.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtkyztrmvv.html

[R39] 重定向标准输出与错误
来源：http://hz.xingfuxueyuan.xyz/gtvaycjyho.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gtmhiohjuz.html

[R40] 追加写日志
来源：http://hz.yj20258.top/gtdyepzgjt.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtrqpimxut.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtnbpnynwc.html

cmd >/dev/null 2>&1
来源：http://hz.hywenlv.cn/gtoggmvdfr.html

[R42] 输入重定向
来源：http://hz.hysaishi.cn/gtslityytx.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtecntmrgd.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtfydgxbwm.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtnhdafuaa.html

[R44] 按修改时间查找
来源：http://hz.zhongyouzk.top/gtgcwjscoq.html

find . -mtime -7 -type f
来源：http://hz.snrcjt.cn/gtnvfbfdxk.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtdyocadhb.html

find . -name "*.tmp" -delete
来源：http://hz.zhengqikj.top/gtavxftcqa.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtpqeoekje.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangkeji.top/gtpauqakxr.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gtbidxashm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtypsiclol.html

[R48] awk 取指定列
来源：http://hz.yangfankeji.com/gthcdmxqzw.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtuqocxhgn.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtowxjnmkh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shangyingyoupin.top/gtgfxecdwv.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtjsbjqpos.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnxiangtu.top/gtjgxgqdhd.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtqejghuyi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.feifeiyinyue.top/gtpcitpivq.html

[R52] 统计行数
来源：http://hz.tanke756.top/gtsbtkypva.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtisfwbipq.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gthzrxjelx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtrlwydndg.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtckiepuif.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtgyqfgncb.html

[R55] 压缩与解压
来源：http://hz.gogol.net.cn/gtalorgzuf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.52xcode.cn/gtohyimruq.html

[R56] 远程拷贝
来源：http://hz.hywenlv.cn/gtuyjesabo.html

scp file user@host:/path/
来源：http://hz.hysaishi.cn/gtsgvldolw.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtgrudeerx.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtezcvppng.html

[R58] 下载文件
来源：http://hz.xinyue.icu/gtwposktdb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yueranfly.top/gthyvgcoiu.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtywjrvblo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangtech.top/gtxhksbpkj.html

[R60] 只看 HTTP 状态码
来源：http://hz.birdmap.top/gtxjvdircn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtvsseyrvv.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangkeji.top/gtlieknjqs.html

df -h;  du -sh *
来源：http://hz.jiagoushi.top/gtciyyksiw.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtupkaqffi.html

du -ah . | sort -rh | head -10
来源：http://hz.hnxiangtu.top/gtalxdtrpi.html

[R63] 内存与进程
来源：http://hz.yuxming.cn/gtavbgamcc.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtmnrptrjl.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtfwzlleoi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuanzhike.top/gtogatzvnr.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtkmlgfohf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtdelxgsrt.html

[R66] 定时任务
来源：http://hz.jinqigfzy.top/gtgwihxkwn.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gtjlnroymz.html

[R67] 生成随机十六进制串
来源：http://hz.iojbl.cn/gthwzoinjy.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gtijzakeph.html

[R68] 计算文件校验值
来源：http://hz.havefunace.top/gtrvdplvis.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtxcxeeveo.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gtfivtozyl.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gttsawguwn.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gtebiznxqk.html

date +%s;  date -d @1700000000
来源：http://hz.yuxming.cn/gtfalzvsoh.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtryvpixzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtmfdopujl.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtwyukqrlf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtxtidfskd.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtyxnpxmgg.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gttvkzhdfk.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtlflsoqdk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuxming.cn/gtzzsnidej.html

[R75] 导出环境变量
来源：http://hz.gotoacloud.top/gtctptjkaz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxinkj.top/gtgztficjl.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtgidoabml.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtfnprficc.html

[R77] 读取用户输入
来源：http://hz.vqdsnc.cn/gtxkepkhjk.html

read -rp "请输入: " ans
来源：http://hz.wangdashe.top/gtuenbztds.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtnnrscbab.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ehwqpu.com/gtbgllyigk.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtvadwajmp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtdyxluppr.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtoendkome.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtfwxsqitm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnsjzdmse.html

S. C / C++ 专题
来源：http://hz.hfpthk.cn/gthboqkegk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthapbfmgk.html

[S01] C：Hello World
来源：http://hz.zhengqikj.top/gtvbkoqzwu.html

#include <stdio.h>
来源：http://hz.guowangkeji.top/gtpoajozmy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtslfeebtv.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gteuudwctq.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtjrcwkuuu.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtusejrgeq.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtnmximmpo.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtlitakpwh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuanzhike.top/gtgsfzuenu.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gtazzlalwl.html


<!-- 参考信息 -->