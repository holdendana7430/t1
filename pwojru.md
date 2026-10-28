代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.haohaochexian.top/gtjlpauafl.html

[Q24] 去重
来源：http://hz.daria6918.cn/gtbyazopxu.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gteozmgjbh.html

[Q25] 只取前 N 条
来源：http://hz.birdmap.top/gtgiokmvyr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.birdmap.top/gtkgjmsncl.html

[Q26] 计数
来源：http://hz.chenlongwang.top/gtubrbpbsg.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gthiraqyia.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtmhzdqrhj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ybcxt.top/gtwgnarfdz.html

[Q28] 求和与平均
来源：http://hz.sysykeji.top/gtdgkiautp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.vqdsnc.cn/gthpmdtrwc.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtjpjhzebv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gthcpqfdvp.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gteciloszi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtuqdgvqww.html

[Q31] 分组后过滤
来源：http://hz.ydjk.org.cn/gtlplujwdk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hammf.cn/gtsbmxgzkm.html

[Q32] 分组拼接字符串
来源：http://hz.cdnleiting.top/gtzumomdpz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtcbtmuqka.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhixingplan.top/gtvyzdpvcv.html

[Q33] 多列分组
来源：http://hz.dianchejie.cn/gtdstgyhos.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenlongwang.top/gtavknyyfz.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtgxkpcnhb.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtrumwmndf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tianlin.xyz/gttzalrsrf.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtxzkcxgfq.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gttbarbdwn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gttqeruwee.html

[Q36] 左连接
来源：http://hz.zhixingplan.top/gtpnkbztdc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gthhvreuyf.html

[Q37] 右连接
来源：http://hz.andypj.xyz/gtdsohvrsi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhoulong.xyz/gtalutqrrx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtnttcacvb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jlsjyb.cn/gtoiunxmuf.html

[Q39] 自连接（查上下级）
来源：http://hz.nwbrower.top/gtmvqphodm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shzxlz.cn/gtsbcfbmca.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtjjatpaqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.0kj1m.cn/gtgtchxxvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tian-w.cn/gtpldavjpd.html

[Q41] 多表连接
来源：http://hz.andypj.xyz/gthleahlwm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtbdutwseh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hfpthk.cn/gtliwbrgit.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gthmldsvlc.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtalhxgqop.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtjsnzcaue.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtsdkbyvqc.html

[Q43] 标量子查询
来源：http://hz.zhiwuduotai.top/gtwdqpobll.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtqlaorwqj.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gttfjwxphi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xingfuxueyuan.xyz/gtknelvaen.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxinkj.top/gtqcoijowc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtpjprzfsn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtaexfqite.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtldkrsfaa.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtmglvsxtj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sxryk.cn/gtbvieimnm.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtvabupqji.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhengqikj.top/gtgswkiarf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuanzx.com/gtawgeodyk.html

[Q49] 更新单行
来源：http://hz.kuanghao11.cn/gtvqrxbppw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gthltrtzqb.html

[Q50] 批量更新
来源：http://hz.haohaochexian.top/gtszvzbaye.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ywan-chungtsiang.top/gtfaacfncx.html

[Q51] 用子查询更新
来源：http://hz.jqgfzy.top/gttxrjuivs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gteulxxcju.html

[Q52] 删除指定行
来源：http://hz.pycfn.com/gtlqndvoyp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gotoacloud.top/gtmehfimew.html

[Q53] 按条件删除
来源：http://hz.sufxvd.cn/gtchspkacq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtdagovwws.html

[Q54] 清空表
来源：http://hz.yvedp.cn/gtuoxtxafz.html

TRUNCATE TABLE logs;
来源：http://hz.daria6918.cn/gtmwtkwhkn.html

[Q55] 排名（并列占位）
来源：http://hz.jiagoushi.top/gtikjusfnd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtuonkygih.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gtmrdchkjb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sufxvd.cn/gttzlnhosb.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtyvmfebmh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtiyrjelpe.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtostonpux.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xinyue.icu/gtdgjatgsk.html

[Q59] 分组内累计
来源：http://hz.0kj1m.cn/gtavmddtuy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtflyabzgr.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtxytlekzv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gtbruvbtpy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gtsdrijigg.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtcparplof.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gthqhuldqj.html

[Q62] 分组占比
来源：http://hz.52xcode.cn/gteufjpibu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtqpwwotmm.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtlyccbwtp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gthyuaksiq.html

[Q64] 提交事务
来源：http://hz.yuanzhike.top/gtdgmhluqt.html

COMMIT;
来源：http://hz.yuxming.cn/gtqfyxyxkn.html

[Q65] 回滚事务
来源：http://hz.daxiang520.top/gtmewqbwrf.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtsqssveux.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtrpjozbau.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtomtqauje.html

[Q67] 设置隔离级别
来源：http://hz.cashguo.top/gtrkfvghkm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtbfbanpqh.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gtbepgoyos.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gterlworvv.html

ROLLBACK TO sp1;
来源：http://hz.guowangkeji.top/gtyzuvbhml.html

[Q69] 查看执行计划
来源：http://hz.daria6918.cn/gtxfvpgqpt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtawmnrcjb.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gttauxzlff.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtudfuzgkf.html

[Q71] 查看建表语句
来源：http://hz.ppjwa.cn/gtbvjicvan.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtqpgwmiyc.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gtelsxzgjy.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtntvfsgug.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gttdmjyhdy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gtmbjyhqgi.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtljjvzfan.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtzijsshap.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gteprsrfzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtipwwrgyk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtlbtkmudp.html

[Q76] 按天统计
来源：http://hz.chenjidiqi.icu/gtnyiknzmg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtqejdswgi.html

[Q77] 时间加减
来源：http://hz.zhixingplan.top/gteuyljxol.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtrbixfjap.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtpjvqtobg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.havefunace.top/gtgcelatej.html

[Q79] 字符串拼接
来源：http://hz.hnqzz.top/gtpkvrvdoa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tian-w.cn/gtywbimlkb.html

[Q80] 字符串截取
来源：http://hz.xziqi.cn/gtkgzwgnfx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shzxlz.cn/gtbzjhwzcq.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gtxuyknkdq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtggbuuwah.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtccwlzjbb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pycfn.com/gtyaaonnyx.html

[Q83] 大小写转换
来源：http://hz.ivvv.top/gtjvzhhrxd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gtpmqsrbqh.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtfqkrujut.html

SELECT TRIM(name) FROM users;
来源：http://hz.guowangkeji.top/gtcxiksfzs.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtwmotuszx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtprwczjsv.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtscvgsvqf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtxeekuict.html

[Q87] JSON 字段做条件
来源：http://hz.cdnleiting.top/gthevldrqc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhiwuduotai.top/gtenrwlshi.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtdsjrqujb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangtech.top/gtiziqprlm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guannengcc.top/gturvendci.html

[Q89] 判断表是否存在
来源：http://hz.cqqwz.cn/gtpxvrvavs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.mhx1999.top/gtqgiuygrl.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtukkomqbk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtqmebxrwu.html

================================================================================
来源：http://hz.jlsjyb.cn/gthlxmbivr.html

R. Bash 专题
来源：http://hz.yonumen.top/gtdyiyshvt.html

================================================================================
来源：http://hz.jqgfzy.top/gtjihzilou.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gtdqfapgfx.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtiuxdbzry.html

set -euo pipefail
来源：http://hz.quarkkingdee.top/gtibjfzwcu.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtnanitvfi.html

name="Tom"; echo "$name"
来源：http://hz.jinqigufen.top/gtpikngryv.html

[R03] 只读变量
来源：http://hz.sufxvd.cn/gthivpltiv.html

readonly PI=3.14
来源：http://hz.cashguo.top/gtyajfuqtb.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gtobpbgrfx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jiagoushi.top/gttyunpalh.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtvbrjdpvi.html

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gtomiijjgi.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtlpzuxzuy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtyaaminvr.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtjbiboatu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtwykscefu.html

[R08] 数值比较
来源：http://hz.0kj1m.cn/gthrfghtkb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gttqnmbane.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtadyehlca.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtzvdhibey.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtynfaeeth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xziqi.cn/gtnuondsye.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtwttzfjho.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gtcysjoqst.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtcsgpeekv.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtquwwuhme.html

*)     echo "未知命令" ;;
来源：http://hz.havefunace.top/gtwropnnkw.html

esac
来源：http://hz.xuanzx.com/gtjuqqdnmv.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gtqjcichpw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtxleugnxy.html

[R13] for 计数循环
来源：http://hz.gzhubu.top/gtbwxrgpvj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenlongwang.top/gtrknceluw.html

[R14] C 风格 for
来源：http://hz.guannengcc.top/gtyihzlsjb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtzhknnltt.html

[R15] while 逐行读文件
来源：http://hz.yj20258.top/gtmmuwnugm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtbucequyd.html

[R16] until 等待条件
来源：http://hz.jinghuilouyu.cn/gtnhjlphpq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigufen.top/gtyvzwdhay.html

[R17] 数组定义与取值
来源：http://hz.nanxinkj.top/gtnrsgnvcp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtgizlvpbe.html

[R18] 遍历数组
来源：http://hz.haohaochexian.top/gtqxhdhaww.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jianghu66.top/gtoukzwdci.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtkenqpkug.html

echo "${#arr[@]}"
来源：http://hz.chenlongwang.top/gtdknyfpji.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtuaxzwdol.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtilihkhkm.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtpcbgwcda.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gthipuljpr.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtsrlsemmj.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtcezidjkc.html

[R23] 字符串替换
来源：http://hz.cheryme.top/gthbrqeioh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtruubyidg.html

[R24] 大小写转换
来源：http://hz.ydzc1.top/gtysftgsxx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtcppahzmd.html

[R25] 去后缀 / 去前缀
来源：http://hz.shuidangran.top/gtmkgevsnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gogol.net.cn/gtrwiqnchp.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtwvepyiud.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gtqcycjexn.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtokukdyok.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtmsgcgvcd.html

[R28] 浮点运算
来源：http://hz.52xcode.cn/gtzqwrtpdw.html

echo "scale=2; 10/3" | bc
来源：http://hz.jlsjyb.cn/gtfxpnparb.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtrtdqezfk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jiagoushi.top/gtzlnnvrjy.html

[R30] 函数返回状态码
来源：http://hz.svipenyu.cn/gtnhukjwbx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydjk.org.cn/gtfzmqbgyb.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtepgkmxrn.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtmgiyyhua.html

[R32] 参数个数校验
来源：http://hz.chenlongwang.top/gtblsnbptu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gtfracvujb.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtnozuxcqi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtdbhovybl.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtxlqwlwtu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtktayejog.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtifbuztph.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtaqhdtnpn.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtxnajqybz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tianlin.xyz/gtrpcnenob.html

[R37] 把输出赋给变量
来源：http://hz.nanxuanxn.top/gtbclazxts.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtqglsnwpb.html

[R38] 管道串联
来源：http://hz.dianchejie.cn/gtidpcntoq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhongyouzk.top/gtxfuvyemc.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gtxfzobrvc.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtjyjskstc.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gthltqtcop.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gtxtnsdwps.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtzzhmcusf.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtjrrxfsdf.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gttfxzskkf.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtrgcumjzb.html

[R43] 按名字查找文件
来源：http://hz.cucudq.cn/gtdendompi.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gtxnzhqfqw.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gtmgstpsju.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtaaodgdrt.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtefxlgxyu.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtxydhqlrk.html

[R46] 递归替换文件内容
来源：http://hz.dianchejie.cn/gtfuhpvzaq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuetiantiany.cn/gtsgjdqttj.html

[R47] sed 单行替换
来源：http://hz.xziqi.cn/gtmayvzirk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtldztvpnt.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtygjxhbvd.html

awk '{print $1, $3}' a.txt
来源：http://hz.ehwqpu.com/gtaieelhuc.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtaavevemh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtcabbwpbl.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtlfcjpxsu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gtbpzbweia.html

[R51] 排序去重取前几
来源：http://hz.aibaodan.cn/gtxzkauhqx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gthrofbwxo.html

[R52] 统计行数
来源：http://hz.hywenlv.cn/gtypckwzwz.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtznohuzev.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtfnkdegaa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gtmyiifzjz.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtlyrlbfac.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gtlxaklgyw.html

[R55] 压缩与解压
来源：http://hz.sxryk.cn/gtbsqsmcrc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenzaomai.com/gtkthbfkav.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtfgrpxdwd.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtsxfjihmw.html

[R57] 远程执行命令
来源：http://hz.zhixingplan.top/gtupbvsctd.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtwzpacprk.html

[R58] 下载文件
来源：http://hz.daxiang520.top/gtkzbtdtbj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuetiantiany.cn/gtpmmlfenv.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtoriszkda.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhiwuduotai.top/gtdkymcfgc.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtgnofnegd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtyeuimuhk.html

[R61] 磁盘占用
来源：http://hz.aibaodan.cn/gtvhfwpvwc.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gtuqbjafcx.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtasxrrxep.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtofmyjfzm.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtvozkpnvk.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gttmqgsswg.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gttvjscraf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gthtyjnxkw.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gttchuztcb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xinyue.icu/gtzcdsndok.html

[R66] 定时任务
来源：http://hz.yongpay.top/gtggypmvdd.html

crontab -e;  crontab -l
来源：http://hz.tian-w.cn/gtghbsbkls.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gthvjxopox.html

openssl rand -hex 16
来源：http://hz.birdmap.top/gttwwojfby.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gtjsyhvmoy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gtjznapvpf.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gtcxxwnwce.html

head -c 16 /dev/urandom | base64
来源：http://hz.ehwqpu.com/gtbiyueleb.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gteoxcirpy.html

date +%s;  date -d @1700000000
来源：http://hz.yj202588.top/gtjygjcndi.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtyckdrwvl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtiglmkoks.html

[R72] 等待端口就绪
来源：http://hz.zhoulong.xyz/gtiggcgpkz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hnxiangtu.top/gtluloaffz.html

[R73] 分割大日志
来源：http://hz.hongshengwenyu.top/gtsayzqrab.html


<!-- 参考信息 -->