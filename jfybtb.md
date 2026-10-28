代发 wailian999

[Q33] 多列分组
来源：http://hz.xingfuxueyuan.xyz/gtjamzkstx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtatpgjvan.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gtcasxbiba.html

SELECT * FROM (
来源：http://hz.aibaodan.cn/gtrsmfrvfa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sysykeji.top/gtxfbmmkta.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtivzxqhhl.html

[Q35] 内连接
来源：http://hz.zhaomingkeji.xyz/gtaltpmtrb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtdlrroaeg.html

[Q36] 左连接
来源：http://hz.meibo888.top/gttnxuyllk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtutnfwasq.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gtkgyjlcts.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gtuxvgwzzq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtbtfybyaq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shzxlz.cn/gtrnpggknm.html

[Q39] 自连接（查上下级）
来源：http://hz.pengpengdd.cyou/gtodysbnzi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.meibo888.top/gtopjdcknj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtsmovvqfm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.feifeiyinyue.top/gtinzotxnd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ywan-chungtsiang.top/gtxbvrczud.html

[Q41] 多表连接
来源：http://hz.0kj1m.cn/gtlbycpajg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtgesgsdco.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cdnleiting.top/gtpvdyestm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtskvyudnb.html

[Q42] 连接条件附加过滤
来源：http://hz.zhixingplan.top/gtzjrnnbel.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtuowfpnmj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fzhhl.top/gtbvcgxlci.html

[Q43] 标量子查询
来源：http://hz.jinghuilouyu.cn/gtgginvmbi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj202588.top/gtpuexypaq.html

[Q44] IN 子查询
来源：http://hz.aizwys.cn/gtnlddzbrx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtuqhmjuql.html

[Q45] EXISTS 判断存在
来源：http://hz.vqdsnc.cn/gtttablyro.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtqxhzphrz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jiagoushi.top/gtthlqnhlb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gtwqrzipiu.html

[Q47] 与平均值比较
来源：http://hz.jinqigufen.top/gtgpcxgcla.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ehwqpu.com/gtyxjpguvy.html

[Q48] CTE 公用表表达式
来源：http://hz.jinghuilouyu.cn/gtdwvmvscm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtrzceoiif.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtbqeeqaij.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtaslvwsqk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydzc1.top/gtuauzziin.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtlkudybcd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dianchejie.cn/gtgjsnvsnu.html

[Q51] 用子查询更新
来源：http://hz.snrcjt.cn/gtvcvskhcx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtsiosqqyc.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtozszchjb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangtech.top/gttimhhzot.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtbzmwgtmt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gtxczmemga.html

[Q54] 清空表
来源：http://hz.smart0.xyz/gtvmotopaq.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtylzxanxf.html

[Q55] 排名（并列占位）
来源：http://hz.tian-w.cn/gtlofqukow.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dianchejie.cn/gtqvppzmjq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shzxlz.cn/gtwlwvxdrf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhixingplan.top/gtwnerckho.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtjkffvgxi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.9152youxi.cn/gtwutmimlr.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtadtnjmaj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ehwqpu.com/gttyfbuqxi.html

[Q59] 分组内累计
来源：http://hz.tanke756.top/gtmjcxunhe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gteftjhfpy.html

[Q60] 取上一行 / 下一行
来源：http://hz.9152youxi.cn/gtphqxzkgx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtwoetaequ.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenjidiqi.icu/gtjmifbipb.html

[Q61] 移动平均
来源：http://hz.zhixingplan.top/gtaxwotebn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cashguo.top/gtlpxwhkac.html

[Q62] 分组占比
来源：http://hz.iojbl.cn/gtvjtaaflc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtkabkhymj.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gttsqikgkw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gttmamoikr.html

[Q64] 提交事务
来源：http://hz.jiagoushi.top/gtfzdulpcl.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtpuzieeta.html

[Q65] 回滚事务
来源：http://hz.pycfn.com/gtupiymmvp.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtmdrddllv.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtafimsewx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtuxbcmvpk.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtffceossv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtljjfppay.html

[Q68] 保存点
来源：http://hz.yangfankeji.com/gtzlsicbke.html

SAVEPOINT sp1;
来源：http://hz.jinyuanbaomall.cn/gtkwvzjkxc.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtrvbktbqj.html

[Q69] 查看执行计划
来源：http://hz.jyoumei.cn/gtjjaskqdb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtnjknoyzf.html

[Q70] 更新统计信息
来源：http://hz.chenjidiqi.icu/gtinqdzywk.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtdxrktxdr.html

[Q71] 查看建表语句
来源：http://hz.havefunace.top/gtkqtytkmn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtvujrpwxc.html

[Q72] 查看索引
来源：http://hz.tianlin.xyz/gtvtkstepo.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtzlrzxnbi.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gtodexgizd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtgkzgrxym.html

[Q74] 强制使用索引
来源：http://hz.chenzaomai.com/gtorlwfrjf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gthlheshkw.html

[Q75] 日期格式化
来源：http://hz.tian-w.cn/gtfipoincu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jlsjyb.cn/gtvskvausl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtyuzyafja.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtkbdrwicp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sysykeji.top/gtgrvwaydf.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtgjjqiofu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangtech.top/gtkguypcwu.html

[Q78] 当前时间
来源：http://hz.tanke756.top/gteeopclgl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gttnibzpmx.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtaeehphlf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gtxdswtzls.html

[Q80] 字符串截取
来源：http://hz.ppjwa.cn/gtktjjxsuy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gotoacloud.top/gtibadigcx.html

[Q81] 字符串替换
来源：http://hz.mhx1999.top/gteqhybuni.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtqkdyesbn.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtwroljhhf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtjqlhlqkq.html

[Q83] 大小写转换
来源：http://hz.redwolf501.top/gtkgywzair.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aibaodan.cn/gtseirdpkj.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtteubajww.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtsqryvrzb.html

[Q85] 数值取整
来源：http://hz.yonumen.top/gtptwlsovh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xinyue.icu/gtirvmzpkm.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxinkj.top/gtcmdrghlz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.vqdsnc.cn/gtemzlwcrf.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtmpskihtg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.pycfn.com/gtlpzrlhzn.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtmxlhbdep.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sweek.top/gtcoonrvfi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtqtdswcpr.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtwclcauqz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jyoumei.cn/gtryeioasd.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gthknoxvht.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtqbkeyrpv.html

================================================================================
来源：http://hz.yangfankeji.com/gtjrnxenva.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtmxeircyi.html

================================================================================
来源：http://hz.cheryme.top/gtngzfwmyh.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtgtdhutfl.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtmynvwlmd.html

set -euo pipefail
来源：http://hz.iojbl.cn/gtgxvxhsox.html

[R02] 变量赋值与使用
来源：http://hz.nanxuanxn.top/gtqylabgfh.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gtyiymicnc.html

[R03] 只读变量
来源：http://hz.andypj.xyz/gtxzvzpmxi.html

readonly PI=3.14
来源：http://hz.zhaomingkeji.xyz/gtrfvvtvpq.html

[R04] 位置参数
来源：http://hz.yj20258.top/gtbouvutfq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gtpryceeoq.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtzpljigqn.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtlwbwqdfp.html

[R06] 判断命令是否存在
来源：http://hz.jianghu66.top/gtksczwkvv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj202588.top/gtqicspcfv.html

[R07] if 判断文件
来源：http://hz.tanke756.top/gtizpumjoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cdnleiting.top/gtbidfbaza.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtaxcavwfh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhaomingkeji.xyz/gtfbesbtqc.html

[R09] 字符串比较
来源：http://hz.c1oappe.top/gttmkvkcjm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtdphvlvvk.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gtkeqskslr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pycfn.com/gtyxihmlvk.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gtigbcpizx.html

case "$1" in
来源：http://hz.xuanzx.com/gtddexwhep.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gtmfueurdi.html

stop)  echo "停止" ;;
来源：http://hz.ybcxt.top/gtdiszikgr.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtxzqccxep.html

esac
来源：http://hz.xziqi.cn/gtarowunxe.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtaztlqzjp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shuidangran.top/gtsajhkfyn.html

[R13] for 计数循环
来源：http://hz.dianchejie.cn/gtkremkhtz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cqqwz.cn/gtkckxbzbu.html

[R14] C 风格 for
来源：http://hz.ydjk.org.cn/gtlewtgibx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gtmxyxjdqd.html

[R15] while 逐行读文件
来源：http://hz.yongpay.top/gtufyrhjsc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtayxrrqzo.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gtkhtniopi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtvesakatq.html

[R17] 数组定义与取值
来源：http://hz.dashuyun.cn/gtopspwitc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guannengcc.top/gtawtlpmuk.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtlcaomlhy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.iojbl.cn/gtfterclyg.html

[R19] 数组长度
来源：http://hz.jinghuilouyu.cn/gtlsfsoipi.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gtuxsxpmeg.html

[R20] 关联数组（字典）
来源：http://hz.0kj1m.cn/gtxlgwsois.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtywgbcnhk.html

[R21] 字符串长度
来源：http://hz.shangyingyoupin.top/gtfwzyhtvt.html

echo "${#s}"
来源：http://hz.mhx1999.top/gtkznbmfbo.html

[R22] 截取子串
来源：http://hz.dianchejie.cn/gtvpkcnvyp.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtrhbhbwho.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtjrnnshau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xingfuxueyuan.xyz/gtwzmschlt.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtergokpjs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gtwkhvimti.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtjeskynwj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxuanxn.top/gtenaarldd.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtsktokemq.html

now=$(date +%F); echo "$now"
来源：http://hz.wangdashe.top/gttycjhtuw.html

[R27] 算术展开
来源：http://hz.chenlongwang.top/gtugyotmra.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtqrpxpxdb.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtrorkckap.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtmxtlposu.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gtdvagrtml.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangdashe.top/gtcexvkigv.html

[R30] 函数返回状态码
来源：http://hz.yongpay.top/gtoiabjcod.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gthkkbrwsz.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtwbavrikf.html

f() { local x=1; echo "$x"; }
来源：http://hz.sweek.top/gttpksyccg.html

[R32] 参数个数校验
来源：http://hz.guannengcc.top/gtyxhyeqaq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtqukldbqb.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gtviqfltmy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtbdvbwhhq.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gtjqjxtmrl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gthacdqgod.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gtfwpipeoa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gtptduiryv.html

[R36] 并发执行多个任务
来源：http://hz.cashguo.top/gtjriwrukz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtnubtfhqn.html

[R37] 把输出赋给变量
来源：http://hz.ydzc1.top/gtdajnuajb.html

files=$(ls -1)
来源：http://hz.zhijiandao.cn/gtnttwehnc.html

[R38] 管道串联
来源：http://hz.zdqjudy.top/gtcwfbkjlg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hysaishi.cn/gtgzykqbpm.html

[R39] 重定向标准输出与错误
来源：http://hz.fzhhl.top/gtsenjjqxs.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtsiycilkg.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gtdhdqmsup.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtzxacpbbm.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtlizphorr.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtgwmbjbif.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtbczkxxua.html

wc -l < a.txt
来源：http://hz.smart0.xyz/gtopmsifdo.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gttgeyurdo.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtbmiybmmp.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gthcjrwpao.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtlxlyslso.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtyneiuzto.html

find . -name "*.tmp" -delete
来源：http://hz.nanxinkj.top/gtvzpkodbc.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtfastdtlp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtkgjqweuu.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtcimuntdh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgufenzy.top/gtcdkrwvkc.html

[R48] awk 取指定列
来源：http://hz.chenlongwang.top/gtjbrcebzn.html

awk '{print $1, $3}' a.txt
来源：http://hz.ehwqpu.com/gtijyfkjvi.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtmelbmzwm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sysykeji.top/gtvbkmhqcs.html

[R50] awk 求和
来源：http://hz.jinyuanbaomall.cn/gtiqrtayxt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtevhyofbw.html

[R51] 排序去重取前几
来源：http://hz.yuanzhike.top/gtmpoxvvnx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtowszixst.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtibmgyvzd.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gthapdwtji.html

[R53] 查看文件头与实时尾
来源：http://hz.hfpthk.cn/gtprldglfh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtkulyvbun.html

[R54] 比较两个文件
来源：http://hz.ydjk.org.cn/gtrvdnkivb.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gteswdaeyl.html

[R55] 压缩与解压
来源：http://hz.wangshuangyany.cn/gtaiikrxua.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangdashe.top/gthultacqw.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gtmwdvsign.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gthubbkjkf.html

[R57] 远程执行命令
来源：http://hz.feifeiyinyue.top/gtsmywqwnr.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gtkftwziiy.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtqjkqeehb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gtxaebbdfl.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtygkbjzge.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtbrbjiini.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gtmalhbbjs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gtcjoepnls.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtmqxlangn.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtjndwozzu.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtrdwcghoc.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtkhkxqqhn.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtxihzeunu.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtsvjtsdvw.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtsqnwikdp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtwkrkeqij.html

[R65] 查看端口占用
来源：http://hz.gaohongyu789.top/gthnkudehf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtlbcpypmr.html

[R66] 定时任务
来源：http://hz.9152youxi.cn/gtrzojcjav.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gttfaritvr.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangkeji.top/gtgykhskgv.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtcfncqymt.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gttycoqvib.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cashguo.top/gtjiqwtlzs.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangtech.top/gtgdtgzccu.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtkndmfkxr.html

[R70] 时间戳与互转
来源：http://hz.xingfuxueyuan.xyz/gtayrwttwi.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gtbhpykblu.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtwyqdaboi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gtmsxckgse.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtvkwfptzd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.svipenyu.cn/gtzfjfzjph.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gtuzaqcfom.html

split -l 1000 big.log part_
来源：http://hz.chenlongwang.top/gtvykkbced.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtpyvhtrwy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhixingplan.top/gtbaiqdjkz.html

[R75] 导出环境变量
来源：http://hz.c1oappe.top/gtsjdzjuku.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xziqi.cn/gttydykods.html

[R76] 使用临时文件
来源：http://hz.dianchejie.cn/gtcoctzhml.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtjjxneyhq.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtgrbuwjxc.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtutkkjerh.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gttangmrcy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtkceoxkoz.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gtpzptjnwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtkofthnid.html

[R80] 查看脚本执行耗时
来源：http://hz.yuxming.cn/gthbvqusze.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtsfkyxnkv.html

================================================================================
来源：http://hz.zycfv.cn/gtvlnkqthg.html

S. C / C++ 专题
来源：http://hz.vqdsnc.cn/gtkzebfmyz.html

================================================================================
来源：http://hz.ivvv.top/gtbuchkcrt.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtyvjgjydq.html

#include <stdio.h>
来源：http://hz.nanxinkj.top/gttzoxpcrz.html


<!-- 参考信息 -->