代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.zhoulong.xyz/gtdnkrmzmc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.birdmap.top/gtcxxjsizx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hongshengwenyu.top/gtkdlxsdns.html

[Q15] 查询全部
来源：http://hz.yonumen.top/gtvgkosftm.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtcesltkbu.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtmazgiefv.html

SELECT id, name FROM users;
来源：http://hz.hywenlv.cn/gtjnskhbwh.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gtppuospzs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hywenlv.cn/gtpqueotwm.html

[Q18] 模糊匹配
来源：http://hz.cheryme.top/gtycwlwvvx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.smart0.xyz/gttkptfsuc.html

[Q19] 范围查询
来源：http://hz.zhengqikj.top/gtkzewyuiz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cashguo.top/gtxgntyxbk.html

[Q20] IN 列表
来源：http://hz.316326.xyz/gtloedwhoa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtazrjpbss.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gtemvfepvg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gtvjkocjnq.html

[Q22] 排序
来源：http://hz.meibo888.top/gtkviceceh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtunzmsltb.html

[Q23] 分页
来源：http://hz.hnqzz.top/gtgngrwroq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtwwttqtbw.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gtlewpqjys.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtwxiztyag.html

[Q25] 只取前 N 条
来源：http://hz.feifeiyinyue.top/gttpugiqrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zdqjudy.top/gtmolvhjey.html

[Q26] 计数
来源：http://hz.dashuyun.cn/gtnkfkaacp.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenlongwang.top/gtqivjgyca.html

[Q27] 条件计数
来源：http://hz.ybcxt.top/gtxfosevnv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guannengcc.top/gthnyftful.html

[Q28] 求和与平均
来源：http://hz.redwolf501.top/gtupbqhdkc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gttsioxbky.html

[Q29] 最大最小值
来源：http://hz.nwbrower.top/gtxzueuuic.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydzc1.top/gtcclncvjb.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtmgbefcqz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.redwolf501.top/gtmhxgpmpi.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gtsbzqgutr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtdkohcegs.html

[Q32] 分组拼接字符串
来源：http://hz.chenjidiqi.icu/gtltmuxdcr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gttvifsryz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtbqgzqzgs.html

[Q33] 多列分组
来源：http://hz.pycfn.com/gtphnfrdnz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangtech.top/gtdrfokpgk.html

[Q34] 每组取第一条
来源：http://hz.smart0.xyz/gtkwfmxvrr.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gthyhirunf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gthkjnpgrn.html

) t WHERE rn = 1;
来源：http://hz.c1oappe.top/gteqpsefon.html

[Q35] 内连接
来源：http://hz.hysaishi.cn/gtuvvhquqt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtpwvniqmw.html

[Q36] 左连接
来源：http://hz.zhixingplan.top/gtbpxkcdov.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtnwmixwyt.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtahhumfgd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zycfv.cn/gtkqqermwg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtjqbvfthv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nwbrower.top/gtamxaqdem.html

[Q39] 自连接（查上下级）
来源：http://hz.hysaishi.cn/gttmjdpcts.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hysaishi.cn/gtpukcurfy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtogqleuve.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtwsmkvzhn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sysykeji.top/gtiajgfbfl.html

[Q41] 多表连接
来源：http://hz.xinyue.icu/gtpktssinu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dianchejie.cn/gtpewaxmwf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinghuilouyu.cn/gtjghbpfto.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tian-w.cn/gtilcdpkad.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtuofapmui.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgufenzy.top/gtfszfipya.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gtmiklagpx.html

[Q43] 标量子查询
来源：http://hz.jinqigfzy.top/gtbibnsvwm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gttngxggnf.html

[Q44] IN 子查询
来源：http://hz.jinghuilouyu.cn/gtsyazafsb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gtbnkiftaf.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtebwohkzc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtqfizibrw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hongshengwenyu.top/gtdsetvjim.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtcsgxyjlf.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtylxqbvvs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtltrrdalj.html

[Q48] CTE 公用表表达式
来源：http://hz.hywenlv.cn/gtjmgbapyu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.feifeiyinyue.top/gtffwfzxjp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenlongwang.top/gtjkqrbbhp.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtslltqkzr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jianghu66.top/gtafrtabiz.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtfrjsccnk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tanke756.top/gtzjtlyjdr.html

[Q51] 用子查询更新
来源：http://hz.xziqi.cn/gtulddkqju.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtjmbpatsj.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtjicvuhdi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtivpuugyg.html

[Q53] 按条件删除
来源：http://hz.yongpay.top/gtouuttqiz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ppjwa.cn/gtooaalvob.html

[Q54] 清空表
来源：http://hz.dashuyun.cn/gtgfwpjdzu.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gthazhcqke.html

[Q55] 排名（并列占位）
来源：http://hz.ivvv.top/gtvsxrdzlt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangtech.top/gtjeqgkutk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.mhx1999.top/gtauqjnzij.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtrtinhnhj.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtfmffutsg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sufxvd.cn/gtbamxkcez.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gthprxsfdm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtxsjfkpjf.html

[Q59] 分组内累计
来源：http://hz.xuetiantiany.cn/gttwiywohz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.9152youxi.cn/gtxczketnb.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258888.top/gtgmuzgwkd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.redwolf501.top/gtjuroiubm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sufxvd.cn/gtkwrshlqr.html

[Q61] 移动平均
来源：http://hz.316326.xyz/gtljwyegjf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sweek.top/gtpwdsztrj.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gttvjqdwcw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gttkwfvkyw.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtqdqzzizx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtlzhggipt.html

[Q64] 提交事务
来源：http://hz.meibo888.top/gtkqqboumv.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtfmgnllyb.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtivhxiidb.html

ROLLBACK;
来源：http://hz.guowangkeji.top/gtfphbnfcw.html

[Q66] 行锁查询
来源：http://hz.wangshuangyany.cn/gteafbwkdu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtxytfbaff.html

[Q67] 设置隔离级别
来源：http://hz.zdqjudy.top/gtjqdhobgt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.mhx1999.top/gtucovgpji.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtdplkmssp.html

SAVEPOINT sp1;
来源：http://hz.hammf.cn/gtaxhwtoye.html

ROLLBACK TO sp1;
来源：http://hz.haohaochexian.top/gtxsiezwoi.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtszsjfzpr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtxngndoyj.html

[Q70] 更新统计信息
来源：http://hz.xylfe.cn/gtvrkybewv.html

ANALYZE TABLE users;
来源：http://hz.yueranfly.top/gtiqaumrlw.html

[Q71] 查看建表语句
来源：http://hz.yueranfly.top/gtksrtqevf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtcbeqmgsb.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gtukrxklae.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtjfehaslx.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gtdrcmxffi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yangfankeji.com/gtwyfjgaat.html

[Q74] 强制使用索引
来源：http://hz.hammf.cn/gtyjhjkwuo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gtpalrcgfo.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtzjxhwapl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtamkeregh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtleiyzsvv.html

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gtcqtvimol.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtmakfsmgs.html

[Q77] 时间加减
来源：http://hz.hammf.cn/gtqhogwpmo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gtzbcasseb.html

[Q78] 当前时间
来源：http://hz.c1oappe.top/gtznxdrxcb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtmxdebjdd.html

[Q79] 字符串拼接
来源：http://hz.yvedp.cn/gtwkjmubqt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jiagoushi.top/gtcodsncfh.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gtswofczpg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangtech.top/gtcegpkzmi.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtwtliqfho.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtwlljvpno.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtscufnznx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ivvv.top/gtulxoxgpk.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtkjlrzlel.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gttphstpcy.html

[Q84] 去除首尾空格
来源：http://hz.fengsongda.top/gtnoqndosf.html

SELECT TRIM(name) FROM users;
来源：http://hz.iojbl.cn/gtjxarudfi.html

[Q85] 数值取整
来源：http://hz.havefunace.top/gtotsejned.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtadpabucc.html

[Q86] 读取 JSON 字段
来源：http://hz.gaohongyu789.top/gtbhghgrub.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtckkdnyng.html

[Q87] JSON 字段做条件
来源：http://hz.quarkkingdee.top/gtkohdzwvx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gteulkhjmj.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinghuilouyu.cn/gtaiuuyyou.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtfcgeuahw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pengpengdd.cyou/gtbmiqksvc.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtnafcqqlm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.0kj1m.cn/gtlgcctyxb.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtzmnvohxy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.pengpengdd.cyou/gtoacdjnrb.html

================================================================================
来源：http://hz.vqdsnc.cn/gttjeuwjey.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gteirrbfdx.html

================================================================================
来源：http://hz.c1oappe.top/gtwassgcyd.html

[R01] shebang 与严格模式
来源：http://hz.snrcjt.cn/gtxvqwufei.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtcftzmisn.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtlqzhvclb.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtcadcarxl.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gtvhtcifrt.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtqrkbdvxb.html

readonly PI=3.14
来源：http://hz.sweek.top/gtfxeejepi.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtvmncmibr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydjk.org.cn/gtvjiplmyn.html

[R05] 参数默认值
来源：http://hz.ppjwa.cn/gtkqjztfwz.html

name="${1:-default}"
来源：http://hz.tanke756.top/gtvodfirpb.html

[R06] 判断命令是否存在
来源：http://hz.yj202588.top/gtwzjugxib.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258.top/gtiryegpdk.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtnhptpmvi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtwkwfljnn.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gttgagkffg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.svipenyu.cn/gtexojfatb.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtkeuaedpk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxuanxn.top/gtqdszdhue.html

[R10] 正则匹配
来源：http://hz.snrcjt.cn/gtaviuwsef.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.vqdsnc.cn/gtcrfhmqmu.html

[R11] case 多分支
来源：http://hz.yanxiufei.cn/gtueinohbn.html

case "$1" in
来源：http://hz.jianghu66.top/gtqhuysagw.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtkbcoiyri.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gthbsbhuog.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtuiibfkxk.html

esac
来源：http://hz.zdqjudy.top/gtibizadmh.html

[R12] for 遍历文件
来源：http://hz.zhaomingkeji.xyz/gtmxkxcsdp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtfeowgfiy.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtzrylzccl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtyojydted.html

[R14] C 风格 for
来源：http://hz.snrcjt.cn/gtbrbokulz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yueranfly.top/gtpxpqkjvt.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtfibmqkuk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtxbpvounm.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtmqcodqqy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtbznvnvek.html

[R17] 数组定义与取值
来源：http://hz.mhx1999.top/gtnrercujq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daxiang520.top/gtjlfxhuwr.html

[R18] 遍历数组
来源：http://hz.cqqwz.cn/gtzixbagtl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtmsgtmdyr.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtbxxthbmo.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtdjlbbjgh.html

[R20] 关联数组（字典）
来源：http://hz.sufxvd.cn/gtpazghqwg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.birdmap.top/gtcbyhneuu.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtprnxprir.html

echo "${#s}"
来源：http://hz.jinyuanbaomall.cn/gtxewzbwky.html

[R22] 截取子串
来源：http://hz.sweek.top/gtlkxshcjq.html

echo "${s:0:5}"
来源：http://hz.aizwys.cn/gtpsnwirsk.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gteyjexpao.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhengqikj.top/gtzouqkedu.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtiwesedzb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtzjevnkwq.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtxtotofqi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gttuhqpimc.html

[R26] 命令替换
来源：http://hz.cqqwz.cn/gtnreckmgb.html

now=$(date +%F); echo "$now"
来源：http://hz.zhongyouzk.top/gtushhehps.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtjgzcricq.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtljosjddc.html

[R28] 浮点运算
来源：http://hz.yonumen.top/gtzawdojly.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtavjunmya.html

[R29] 定义函数
来源：http://hz.jinqigfzy.top/gtcdqoeqhw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtqklulala.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtgciluswk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtpnwzfglz.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtrxkgfrca.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtziuytvjn.html

[R32] 参数个数校验
来源：http://hz.wangdashe.top/gtqcdjqlbm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtcqcnbzse.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gtvbtflrxk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.9152youxi.cn/gtsjukvhcn.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtlcoklokc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtexqpudzm.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtnxynayuo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtznqkdivs.html

[R36] 并发执行多个任务
来源：http://hz.zycfv.cn/gtyvctyigc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xylfe.cn/gthuopzyyf.html

[R37] 把输出赋给变量
来源：http://hz.daria6918.cn/gtfudegqrr.html

files=$(ls -1)
来源：http://hz.ywan-chungtsiang.top/gtfboshmdt.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtcrfrazzt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nwbrower.top/gtiqtnadou.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtvxnfcdhk.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtynaiuuxi.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtphmexlkc.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtwukjotbj.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gtzkbznoyr.html

cmd >/dev/null 2>&1
来源：http://hz.pycfn.com/gtzorskvux.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gtbukmlufw.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtipoqtqtx.html

[R43] 按名字查找文件
来源：http://hz.gotoacloud.top/gtgsnegeyw.html

find . -name "*.log" -type f
来源：http://hz.yueranfly.top/gtoszxckzl.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtpmethjju.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtcujffdwi.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtlgytcjoj.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtanwzmrrn.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtdyxnkspl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fengsongda.top/gtyvebvbjw.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gttykjcsdd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gtlyvmhgda.html

[R48] awk 取指定列
来源：http://hz.birdmap.top/gtybedinfz.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gttcabpnjr.html

[R49] awk 带条件
来源：http://hz.zdqjudy.top/gtkhqvaqpb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuetiantiany.cn/gtmyakziyu.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtjntckwem.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gogol.net.cn/gtiawgazrk.html

[R51] 排序去重取前几
来源：http://hz.quarkkingdee.top/gtazildalp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yueranfly.top/gtpwbnjbsj.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtblrtvkfe.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtynirxwsl.html

[R53] 查看文件头与实时尾
来源：http://hz.yuxming.cn/gtayekkhks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtcxnjdpnb.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtscaqjgdv.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtfxforhbr.html

[R55] 压缩与解压
来源：http://hz.quarkkingdee.top/gtbvfysjte.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtwasbcsvk.html

[R56] 远程拷贝
来源：http://hz.yueranfly.top/gtsabrbksh.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtjduuqzug.html

[R57] 远程执行命令
来源：http://hz.feifeiyinyue.top/gttdrqrjha.html

ssh user@host 'uptime'
来源：http://hz.nanxinkj.top/gtroknplih.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtetlnzjuv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtkpajbtsx.html

[R59] 发 POST JSON
来源：http://hz.havefunace.top/gtnbrmggys.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtatuixill.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtvxkslxgg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtnszorods.html

[R61] 磁盘占用
来源：http://hz.tian-w.cn/gtgqttzrpf.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtntjoanoo.html

[R62] 找最占空间的文件
来源：http://hz.fzhhl.top/gtveuladoo.html

du -ah . | sort -rh | head -10
来源：http://hz.xinyue.icu/gtxhascqxb.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtamrahvkg.html


<!-- 参考信息 -->