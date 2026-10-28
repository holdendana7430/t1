代发 wailian999

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtkqovcowa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtgrppcbxz.html

[Q37] 右连接
来源：http://hz.sysykeji.top/gtwvpqceam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtwxdlaenc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gtxxvzktve.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pengpengdd.cyou/gtrdyonidp.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gtxixqeytl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.feifeiyinyue.top/gtvrcaqvpm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhaomingkeji.xyz/gtzerbombr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258.top/gtuyouslae.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gthhqfxfoy.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtsnngglay.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhengqikj.top/gtvgbfzosj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtrhpyeelw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxuanxn.top/gtprjhpmyb.html

[Q42] 连接条件附加过滤
来源：http://hz.pycfn.com/gtegunzevr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnqzz.top/gtjltcgxst.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtvtbcyplm.html

[Q43] 标量子查询
来源：http://hz.c1oappe.top/gtdjfxaqsm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtmshlivgk.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtumfmoqzh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj202588.top/gtshplkzhn.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gtainrepkn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yonumen.top/gtablqvlgk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtrppgqyps.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtaxiobbzc.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gtgnvpoclg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtxahhytgd.html

[Q48] CTE 公用表表达式
来源：http://hz.fzhhl.top/gtchyfhxhk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtpoxsmclb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtuuqorbux.html

[Q49] 更新单行
来源：http://hz.hongshengwenyu.top/gtvmrubyjn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtngarrcpq.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtwesnljpj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258888.top/gthiyqheow.html

[Q51] 用子查询更新
来源：http://hz.svipenyu.cn/gtrymtrugu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtkudaxbqt.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gtdwmgrlth.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtfeeyxcly.html

[Q53] 按条件删除
来源：http://hz.ehwqpu.com/gtycezrwjn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ivvv.top/gttlbegwko.html

[Q54] 清空表
来源：http://hz.jqgufenzy.top/gttaoewbzc.html

TRUNCATE TABLE logs;
来源：http://hz.fengsongda.top/gthrrstjbe.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtsynwelzu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cqqwz.cn/gtfsgxpslh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yangfankeji.com/gtzrgiabla.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258888.top/gtjigrozqn.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtfwrcitbs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fengsongda.top/gtekvrsvgy.html

[Q58] 累计求和
来源：http://hz.zhoulong.xyz/gtsqilxxmq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jlsjyb.cn/gtxdouxqoh.html

[Q59] 分组内累计
来源：http://hz.xziqi.cn/gtlhztvydt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ehwqpu.com/gtopgtnyew.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtrortcuag.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtixispcab.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtmpdcecbb.html

[Q61] 移动平均
来源：http://hz.feifeiyinyue.top/gtkmclzxuh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gtsyvqiatc.html

[Q62] 分组占比
来源：http://hz.yuxming.cn/gtbspptrad.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtsxglkizt.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtpchnwfqd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xylfe.cn/gtvmlgzeqc.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gteyxvwplv.html

COMMIT;
来源：http://hz.zycfv.cn/gtipnzivrp.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtthrebqkb.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtoegywnxu.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtxxocfqht.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtfukhopnu.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gtadvejnwv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cheryme.top/gtftcqlmhj.html

[Q68] 保存点
来源：http://hz.zhixingplan.top/gtsvobaimg.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtzjzxuhdm.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtlpawtdkg.html

[Q69] 查看执行计划
来源：http://hz.zhijiandao.cn/gtzommjnji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtbclvoaqu.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtfhqfscty.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gttgfdlxvt.html

[Q71] 查看建表语句
来源：http://hz.0kj1m.cn/gtgntuxggs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.bjfxy.top/gtowenfwfv.html

[Q72] 查看索引
来源：http://hz.yanxiufei.cn/gtkaahzyqm.html

SHOW INDEX FROM users;
来源：http://hz.jqgfzy.top/gtlykulzuc.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gtlgrfayxf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gtkzuadamy.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gtoohnixcz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jianghu66.top/gtaacxfzki.html

[Q75] 日期格式化
来源：http://hz.ydzc1.top/gtxgckrhvf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fengsongda.top/gtbbtjsxys.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hysaishi.cn/gtlhaiwjid.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtouisfksv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtybprrhcj.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gtlfvcmupy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtszqefyer.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtigifhjiw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtvvhnqvjj.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtqmxsvjzo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jianghu66.top/gtirrhxuco.html

[Q80] 字符串截取
来源：http://hz.yonumen.top/gthpaajpnx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtcefosxps.html

[Q81] 字符串替换
来源：http://hz.dashuyun.cn/gtlwgjbdqn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cashguo.top/gtmdiedyfk.html

[Q82] 字符长度与字节长度
来源：http://hz.nwbrower.top/gtjxxffxqy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhoulong.xyz/gtvfdjxnwz.html

[Q83] 大小写转换
来源：http://hz.52xcode.cn/gtlyutxwmi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtmupyuadd.html

[Q84] 去除首尾空格
来源：http://hz.ywan-chungtsiang.top/gtmmgndsuu.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gteuaerhwg.html

[Q85] 数值取整
来源：http://hz.chenlongwang.top/gtpkpnqhrh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guowangkeji.top/gthinleuxz.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtqstftaer.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jiagoushi.top/gttdjonjzh.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gtgtjfonun.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtdlgzxujc.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gtwxyunjue.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gtrvpaigsn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtxmmatqnl.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtdiehbyft.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxuanxn.top/gtzyqodjob.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtmbemjejs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtxjkljrsv.html

================================================================================
来源：http://hz.haohaochexian.top/gtwuxmzbuw.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtacousvxk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmmtqrwwb.html

[R01] shebang 与严格模式
来源：http://hz.aibaodan.cn/gttnzuyump.html

#!/usr/bin/env bash
来源：http://hz.yonumen.top/gtffmqebeb.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtgdphyiws.html

[R02] 变量赋值与使用
来源：http://hz.zhiwuduotai.top/gtqdavduak.html

name="Tom"; echo "$name"
来源：http://hz.daria6918.cn/gtbqmsmxor.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gtzyvbfxxr.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtmknhgeec.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gthjqyyfrb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.vqdsnc.cn/gtvjciuxyr.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtbqkgghpj.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtukdxxjsb.html

[R06] 判断命令是否存在
来源：http://hz.gotoacloud.top/gttrtsbbqh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtekkzcqwl.html

[R07] if 判断文件
来源：http://hz.zhiwuduotai.top/gtzwgfsoom.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnqzz.top/gtgefhtlap.html

[R08] 数值比较
来源：http://hz.svipenyu.cn/gtxknwznje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtgfyhfhhf.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtjswafqqe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shanyushiyangtech.top/gtxozxgzhl.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtgbjgedzd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhixingplan.top/gtmkdvayjp.html

[R11] case 多分支
来源：http://hz.yuanzhike.top/gtknlgtdjt.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtizlsjsdm.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtxhpbkwbw.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gttsluvund.html

*)     echo "未知命令" ;;
来源：http://hz.gotoacloud.top/gtrrcaijlz.html

esac
来源：http://hz.yj20258.top/gtrsdiucrl.html

[R12] for 遍历文件
来源：http://hz.wangshuangyany.cn/gtfewhhomj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.bjfxy.top/gthjqbbilp.html

[R13] for 计数循环
来源：http://hz.zhiwuduotai.top/gtetqysjao.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenzaomai.com/gtudokzkzh.html

[R14] C 风格 for
来源：http://hz.sxryk.cn/gtpamzqdyo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydzc1.top/gtmmoeytjb.html

[R15] while 逐行读文件
来源：http://hz.yvedp.cn/gtdezaunoj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtpcfjyuwm.html

[R16] until 等待条件
来源：http://hz.ydjk.org.cn/gtkhstokku.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gtxhqkunbr.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtfvktqlrp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gtroekomtg.html

[R18] 遍历数组
来源：http://hz.shanyushiyangtech.top/gtfcssomox.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtfmrudsof.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gteltxqhbw.html

echo "${#arr[@]}"
来源：http://hz.cashguo.top/gteskrjcrm.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtnfzeicwq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtprunkcsd.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtmtstpcur.html

echo "${#s}"
来源：http://hz.cashguo.top/gtaixbjfps.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtdxxlkzss.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtklgfkepv.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtewpxehnl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258.top/gtggupsbjd.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtaeiwfqgv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtrqpylhbx.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtqqqnqjxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pycfn.com/gtldyczpcn.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtxtdjwvdw.html

now=$(date +%F); echo "$now"
来源：http://hz.birdmap.top/gtdcdlxgox.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtmytaekmt.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtajospcgh.html

[R28] 浮点运算
来源：http://hz.0kj1m.cn/gtralkffqr.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtrkjcgsai.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gtkpjefyyo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtvjeecqws.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtualhnwuq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gtxgadagwr.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtymydvvab.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtyjciihfn.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtohdvwqno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtighybfrn.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtmvwmedab.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinyuanbaomall.cn/gtrakzehia.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtpqanswdr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtqrepxcco.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtpuntbkzw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtwpdyqigp.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtlpjkzonm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtfjdhhbup.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gtedllzhnh.html

files=$(ls -1)
来源：http://hz.cdnleiting.top/gtypvnqvwz.html

[R38] 管道串联
来源：http://hz.mhx1999.top/gtelzlvkrg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtzwsaoigm.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtzaduqghq.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtcdtntpxm.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gteagnxful.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtztqelvru.html

[R41] 丢弃输出
来源：http://hz.gzhubu.top/gtdbcprftr.html

cmd >/dev/null 2>&1
来源：http://hz.snrcjt.cn/gtjpaszksp.html

[R42] 输入重定向
来源：http://hz.zhijiandao.cn/gtieowhypl.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gtuipnojve.html

[R43] 按名字查找文件
来源：http://hz.hfpthk.cn/gtvjkzncwb.html

find . -name "*.log" -type f
来源：http://hz.52xcode.cn/gtgjiklbdw.html

[R44] 按修改时间查找
来源：http://hz.aizwys.cn/gtivgvavfh.html

find . -mtime -7 -type f
来源：http://hz.cqqwz.cn/gtqfeciikm.html

[R45] 批量删除
来源：http://hz.cashguo.top/gtuikvwmgc.html

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtlvedcnhv.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtufadbhwx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jiagoushi.top/gtlubdjsag.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gtafidilmm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtcbhvqift.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gthrnjtzif.html

awk '{print $1, $3}' a.txt
来源：http://hz.hammf.cn/gtqazkutzi.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtikmrimiz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtcketcmjq.html

[R50] awk 求和
来源：http://hz.xingfuxueyuan.xyz/gtwdoipdtk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtcgcyqedb.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtincsgyev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tanke756.top/gtxdfcriqm.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtgguscxmu.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtbcktitzw.html

[R53] 查看文件头与实时尾
来源：http://hz.ywan-chungtsiang.top/gtpigrewhn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnxiangtu.top/gtpfcyegjz.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtdsiwmhte.html

diff a.txt b.txt
来源：http://hz.nanxinkj.top/gtiybexpyk.html

[R55] 压缩与解压
来源：http://hz.birdmap.top/gtrjgseiep.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yuanzhike.top/gtaamcsqsc.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtblpvwlmr.html

scp file user@host:/path/
来源：http://hz.snrcjt.cn/gtnctukonn.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gtamzhpvzw.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtlngmrueq.html

[R58] 下载文件
来源：http://hz.gzhubu.top/gtjuwlijee.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gtwfylsfkd.html

[R59] 发 POST JSON
来源：http://hz.zhongyouzk.top/gtxxfzcgmp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtlvdgxgyv.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtdkpnzdgq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtvxlxiuzh.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtmbpbssjn.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtuzrkqvqh.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtwjcdubaw.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangkeji.top/gtqqfolpvu.html

[R63] 内存与进程
来源：http://hz.zhoulong.xyz/gtvulbyypx.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtofeodsnv.html

[R64] 结束进程
来源：http://hz.jyoumei.cn/gtpnaycpif.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtsljkvxgb.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtgpseuxty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtrgtydnyf.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtymkktxlr.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtvtfftolf.html

[R67] 生成随机十六进制串
来源：http://hz.jlsjyb.cn/gtzgdgviqk.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtbusirvyd.html

[R68] 计算文件校验值
来源：http://hz.jinqigufen.top/gthsjeuhub.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinghuilouyu.cn/gtcmightzy.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtvrdvfhly.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtzwsvecmm.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtclnovqpm.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtfhzavvyt.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtifpaelyv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtcfhhxgtk.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtzgardycl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258888.top/gtsizlhzgw.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtnnvlptwr.html

split -l 1000 big.log part_
来源：http://hz.jinqigufen.top/gtvukulkyk.html

[R74] 批量重命名
来源：http://hz.gzhubu.top/gtubcgtzen.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinyuanbaomall.cn/gtxqctregu.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtstbdemsx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtfgiryvso.html

[R76] 使用临时文件
来源：http://hz.xinyue.icu/gtlvbwwbja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtijouhguf.html

[R77] 读取用户输入
来源：http://hz.xylfe.cn/gtxjqfnndf.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtlliyjmuu.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtxgrwglwz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dianchejie.cn/gthaqpcnoe.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtcahvbney.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shangyingyoupin.top/gtaiiiprnn.html

[R80] 查看脚本执行耗时
来源：http://hz.quarkkingdee.top/gtzwxspssd.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtmkunnduh.html

================================================================================
来源：http://hz.nanxinkj.top/gtgjptqhvb.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtnzjjlkwp.html

================================================================================
来源：http://hz.hfpthk.cn/gtueuyjctq.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtzknwwszp.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtlncgkufd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.svipenyu.cn/gthmidfmoo.html

[S02] C：变量与格式化输出
来源：http://hz.xuanzx.com/gtelnufqtv.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtzyibmurb.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtbahifwey.html

int x; scanf("%d", &x);
来源：http://hz.xuetiantiany.cn/gtwhxrboro.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtapzhtauk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxinkj.top/gtaxfnjhme.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtjtnlhogz.html


<!-- 参考信息 -->