代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtxbuptoff.html

[Q20] IN 列表
来源：http://hz.yj202588.top/gtgaygymwj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.meibo888.top/gtgdpktzgg.html

[Q21] 空值判断
来源：http://hz.ppjwa.cn/gtkfmxnwht.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtviyitisj.html

[Q22] 排序
来源：http://hz.gaohongyu789.top/gtfmyvrhbt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sxryk.cn/gtxrcqsnwh.html

[Q23] 分页
来源：http://hz.shuidangran.top/gtplcnnajo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtfogytnru.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gttyscdunc.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgfzy.top/gtexnvixpa.html

[Q25] 只取前 N 条
来源：http://hz.chenjidiqi.icu/gtdguwuhoa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhoulong.xyz/gtuureipnv.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtwmobutsf.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtpvmbqdfl.html

[Q27] 条件计数
来源：http://hz.redwolf501.top/gtciwkuekw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinqigufen.top/gtiqcimuvi.html

[Q28] 求和与平均
来源：http://hz.ywan-chungtsiang.top/gtbmvnfwqw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtxipaodti.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gthxduxbpi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sysykeji.top/gtcvzxdcvn.html

[Q30] 分组统计
来源：http://hz.daxiang520.top/gtkbjegepv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gttrcaskyn.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangtech.top/gtzcpfwymf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtuyexjhad.html

[Q32] 分组拼接字符串
来源：http://hz.jqgfzy.top/gtrivwagup.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtloyhnovb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shuidangran.top/gtsgegzvpr.html

[Q33] 多列分组
来源：http://hz.hywenlv.cn/gtyhqkamej.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhaomingkeji.xyz/gtmpijwrot.html

[Q34] 每组取第一条
来源：http://hz.nanxuanxn.top/gtmjotokev.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gtiloprwso.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gteeiyoxaq.html

) t WHERE rn = 1;
来源：http://hz.cqqwz.cn/gtnmvcdscr.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtbetdgvrb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ybcxt.top/gtuzunzyws.html

[Q36] 左连接
来源：http://hz.jinghuilouyu.cn/gtkypdfvhq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtcbmlweml.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtntcgauiu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtdhntljqv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shanyushiyangkeji.top/gtivlkdbuq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuxming.cn/gtbdvtxdsg.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtthjvjkxf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tanke756.top/gtlredjecd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tian-w.cn/gtvgtghorn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtejjegeul.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.vqdsnc.cn/gtimfivkjb.html

[Q41] 多表连接
来源：http://hz.jianghu66.top/gtlccnwiyu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.kuanghao11.cn/gtgipjemyb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hysaishi.cn/gtoertakom.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cucudq.cn/gtnwensxls.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtzyjqyshn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtniwvluhi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtgjhwunfi.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gtydavjpkr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydzc1.top/gtvwmfcnwu.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gtxbmkgelo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhiwuduotai.top/gtwnclzrcw.html

[Q45] EXISTS 判断存在
来源：http://hz.redwolf501.top/gtbihjjlyw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtrreykflv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.snrcjt.cn/gthurnougs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtmmohnqss.html

[Q47] 与平均值比较
来源：http://hz.ybcxt.top/gtzbjhkehq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtknzkqplq.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtxdxhnzqh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cheryme.top/gtqsaefauk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guannengcc.top/gtlalgcrox.html

[Q49] 更新单行
来源：http://hz.zhaomingkeji.xyz/gthpwahllb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xziqi.cn/gtirlptojk.html

[Q50] 批量更新
来源：http://hz.sweek.top/gtchmbgrgu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shuidangran.top/gtbynknlux.html

[Q51] 用子查询更新
来源：http://hz.hammf.cn/gtogzcjydz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj20258888.top/gtnsighttx.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtkeqswazy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtjybztqka.html

[Q53] 按条件删除
来源：http://hz.shanyushiyangkeji.top/gtdxqwgplh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sweek.top/gtxpwoxfuw.html

[Q54] 清空表
来源：http://hz.gaohongyu789.top/gtrlfvkrol.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtdazsejpr.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtwojpqwkh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.sweek.top/gtupevsexw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtzzvtlllk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangdashe.top/gtnvduaonj.html

[Q57] 行号
来源：http://hz.yanxiufei.cn/gtciuhvmdy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtlpcslkbj.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gtejtqapnh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gthdommggb.html

[Q59] 分组内累计
来源：http://hz.zhaomingkeji.xyz/gtuquqntxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhixingplan.top/gtzjqfpmna.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtifmgoipg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gzhubu.top/gtrdepbusp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.52xcode.cn/gtjuieacmi.html

[Q61] 移动平均
来源：http://hz.yangfankeji.com/gtutqsndxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtdyexxkhp.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gttjodlkic.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.aizwys.cn/gtyakejfay.html

[Q63] 开启事务
来源：http://hz.shanyushiyangkeji.top/gtinrlywqb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangdashe.top/gteywmsdlx.html

[Q64] 提交事务
来源：http://hz.yueranfly.top/gtyrbwccds.html

COMMIT;
来源：http://hz.sufxvd.cn/gtbcvachbu.html

[Q65] 回滚事务
来源：http://hz.52xcode.cn/gtcmjjqoum.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtvnknmjgl.html

[Q66] 行锁查询
来源：http://hz.52xcode.cn/gtnkokkhpf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtofbrtwdu.html

[Q67] 设置隔离级别
来源：http://hz.xuanzx.com/gtxkoxsbkt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gtovgigfxx.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtjswwgaej.html

SAVEPOINT sp1;
来源：http://hz.52xcode.cn/gtzzupujqk.html

ROLLBACK TO sp1;
来源：http://hz.yongpay.top/gteyppxvcj.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtkfaoyaho.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258888.top/gtkvrhlsmv.html

[Q70] 更新统计信息
来源：http://hz.feifeiyinyue.top/gtlwevcisj.html

ANALYZE TABLE users;
来源：http://hz.zhixingplan.top/gtdpotovof.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtcfugcmrl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtbkszamhc.html

[Q72] 查看索引
来源：http://hz.jyoumei.cn/gtvofioizh.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtpmzwmpch.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtcmdejsgc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ivvv.top/gtritwaadc.html

[Q74] 强制使用索引
来源：http://hz.wangdashe.top/gtywazesit.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtmpwnajlr.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtsazxjgbd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtkldlnlty.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtequebrvo.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gtujqmflbq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtwiwsqgrf.html

[Q77] 时间加减
来源：http://hz.zhoulong.xyz/gtefervbif.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtzdyrcexy.html

[Q78] 当前时间
来源：http://hz.fzhhl.top/gticvospog.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtmvasnniq.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtmhcbavvb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gthyqxgyzi.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtchyrheaq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258888.top/gtixjuuydo.html

[Q81] 字符串替换
来源：http://hz.pengpengdd.cyou/gtcxwgwpef.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtrgnhytjx.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtgqdedscd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigfzy.top/gthfvjeohj.html

[Q83] 大小写转换
来源：http://hz.jyoumei.cn/gtrvbqcqfx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhongyouzk.top/gtpbcqxkpo.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtwtywrhih.html

SELECT TRIM(name) FROM users;
来源：http://hz.yangfankeji.com/gtmutppyhj.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtcvkzkqck.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gttjbsrtas.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtgnizonhe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gtyvowkzqi.html

[Q87] JSON 字段做条件
来源：http://hz.cashguo.top/gtaifevdtc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtkwnsyhbi.html

[Q88] 行转列（条件聚合）
来源：http://hz.ppjwa.cn/gtfuwkyemx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tian-w.cn/gtjzpudyza.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhengqikj.top/gtbehqvlnr.html

[Q89] 判断表是否存在
来源：http://hz.ppjwa.cn/gtyfxtyfac.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tian-w.cn/gtogvrhehs.html

[Q90] 生成序号列
来源：http://hz.smart0.xyz/gtpabzqmxi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtzxukajrh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbdhltzti.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtrfntksqe.html

================================================================================
来源：http://hz.52xcode.cn/gtpwkgltpf.html

[R01] shebang 与严格模式
来源：http://hz.zhaomingkeji.xyz/gtdnmzivrb.html

#!/usr/bin/env bash
来源：http://hz.vqdsnc.cn/gtnsegjfvl.html

set -euo pipefail
来源：http://hz.jianghu66.top/gtrevacjid.html

[R02] 变量赋值与使用
来源：http://hz.ppjwa.cn/gtvgnnxxsm.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtncvkmxay.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtldmeluta.html

readonly PI=3.14
来源：http://hz.yanxiufei.cn/gtuhaqajyz.html

[R04] 位置参数
来源：http://hz.shzxlz.cn/gthiuckvln.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtzrwdzpnt.html

[R05] 参数默认值
来源：http://hz.aibaodan.cn/gtcupkrjnc.html

name="${1:-default}"
来源：http://hz.snrcjt.cn/gtaxtdmkrj.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtkosvkrbu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhoulong.xyz/gtjzlhfuca.html

[R07] if 判断文件
来源：http://hz.birdmap.top/gtlsluwndp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtlykxkawk.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtscjrjbcl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhoulong.xyz/gtardbwdwr.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtfzdikcku.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtflykhxep.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gteeawldbd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtnxjooupk.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtsunvacvi.html

case "$1" in
来源：http://hz.guannengcc.top/gtnguctuhf.html

start) echo "启动" ;;
来源：http://hz.aibaodan.cn/gtmuiyrqia.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtkigopuxu.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtqotowchv.html

esac
来源：http://hz.hnxiangtu.top/gtqitbzhft.html

[R12] for 遍历文件
来源：http://hz.sysykeji.top/gtmhxmchun.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhiwuduotai.top/gtdbdcfthr.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtqziprwog.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtfipesxyr.html

[R14] C 风格 for
来源：http://hz.hfpthk.cn/gtbuvsrprz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.smart0.xyz/gtlwhczvmp.html

[R15] while 逐行读文件
来源：http://hz.ydzc1.top/gtucxeinee.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtxmzoobie.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtekikxqiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtkypbmfnj.html

[R17] 数组定义与取值
来源：http://hz.nanxuanxn.top/gtnhqzizkz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jianghu66.top/gtjqyficor.html

[R18] 遍历数组
来源：http://hz.jinqigfzy.top/gtlnujgeyp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gzhubu.top/gtqfemdtmt.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gtviihryfs.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtfzyskrdu.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtjphpyoig.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gtujlqwazr.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtxdiayooy.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtcsmrijrq.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtxpabgplb.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtsyzbsssv.html

[R23] 字符串替换
来源：http://hz.hongshengwenyu.top/gtneqcehkg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhixingplan.top/gtbbpovuzv.html

[R24] 大小写转换
来源：http://hz.quarkkingdee.top/gttsfjqqwb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtyvejkeds.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtzxxbdvck.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gttcqxwjfn.html

[R26] 命令替换
来源：http://hz.sweek.top/gtyesswvat.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtkiyplcti.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtdgkeswnu.html

echo $((1 + 2 * 3))
来源：http://hz.yueranfly.top/gtlhleptiw.html

[R28] 浮点运算
来源：http://hz.tianlin.xyz/gttvtynmwi.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangshuangyany.cn/gtqeucrwlo.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtqubrbskz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangkeji.top/gtsivtxqtw.html

[R30] 函数返回状态码
来源：http://hz.52xcode.cn/gtmrvayfvs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.havefunace.top/gtexjmttbb.html

[R31] 局部变量
来源：http://hz.shanyushiyangtech.top/gtxcezzqfd.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gtcmizjgtr.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtbdshipii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtsjyleisp.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gtzjcigdkk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgufenzy.top/gtrosodicm.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtabyqnagd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtmhojcujs.html

[R35] 后台执行并等待
来源：http://hz.aibaodan.cn/gtyrullwel.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenzaomai.com/gtpldwmopo.html

[R36] 并发执行多个任务
来源：http://hz.yvedp.cn/gtujdnpfff.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gttrnhkzio.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtczdflpho.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gtyjgonnwq.html

[R38] 管道串联
来源：http://hz.cashguo.top/gtleeviysy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj202588.top/gtqqwwgcvq.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtabjvjdwp.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtrranljhl.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gttjjaspvc.html

echo "log" >> out.log
来源：http://hz.chenzaomai.com/gtvoxnzuny.html

[R41] 丢弃输出
来源：http://hz.yangfankeji.com/gtvpqdvehg.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtlsfqixzj.html

[R42] 输入重定向
来源：http://hz.aizwys.cn/gtliqlpiyt.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gtnotnjzjg.html

[R43] 按名字查找文件
来源：http://hz.yonumen.top/gtybywidnb.html

find . -name "*.log" -type f
来源：http://hz.jiagoushi.top/gtczaqfmsk.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtqzexblqc.html

find . -mtime -7 -type f
来源：http://hz.yuanzhike.top/gtanymdpin.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gthfqgkgct.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtonwaerak.html

[R46] 递归替换文件内容
来源：http://hz.zhiwuduotai.top/gthniewfiu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtkwqcmkxo.html

[R47] sed 单行替换
来源：http://hz.meibo888.top/gthqzvlqwy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hongshengwenyu.top/gtfwbfpqtg.html

[R48] awk 取指定列
来源：http://hz.hongshengwenyu.top/gtuvdejrke.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtxctdebtb.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtwrmbbhdy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aizwys.cn/gtxefdbmll.html

[R50] awk 求和
来源：http://hz.tian-w.cn/gtczknwvxa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gthtbwgakw.html

[R51] 排序去重取前几
来源：http://hz.daxiang520.top/gthygkmkth.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gttzagelny.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gttmzoixph.html

wc -l a.txt
来源：http://hz.chenzaomai.com/gtgxgdzhei.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtdhxsszqc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtbqhnfmnq.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gtpedfwijh.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gttxdvdzco.html

[R55] 压缩与解压
来源：http://hz.jyoumei.cn/gtgqsayfot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gtesnxpnur.html

[R56] 远程拷贝
来源：http://hz.c1oappe.top/gtivzjbanm.html

scp file user@host:/path/
来源：http://hz.snrcjt.cn/gtmprwassp.html

[R57] 远程执行命令
来源：http://hz.dianchejie.cn/gtvfboskyk.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtflshmzns.html

[R58] 下载文件
来源：http://hz.zhixingplan.top/gtzlcpgmpg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtkxaepomu.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtkprecaio.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtbqqlewld.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtpfewytbu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hywenlv.cn/gtcfzkqids.html

[R61] 磁盘占用
来源：http://hz.hongshengwenyu.top/gtktfcsviq.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtwrcfcnkr.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtglxstmtn.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtjiruxztc.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtkrjffxaa.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gthgnsgleb.html

[R64] 结束进程
来源：http://hz.jqgufenzy.top/gtlrffwysm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtwsavfkgl.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtwwokmcdl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtpahsbgiw.html

[R66] 定时任务
来源：http://hz.hammf.cn/gtfoeotcoz.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gthodvwuiq.html

[R67] 生成随机十六进制串
来源：http://hz.nanxuanxn.top/gtdfihnzeg.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtesrtfxdc.html

[R68] 计算文件校验值
来源：http://hz.jinqigufen.top/gtkdsozgly.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtfkzismkn.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtfrtcoobv.html


<!-- 参考信息 -->