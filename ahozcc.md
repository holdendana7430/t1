代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zycfv.cn/gtliwexihf.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gtyjdistmc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xinyue.icu/gtrwyfdhvu.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtgajppzld.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cdnleiting.top/gtuiedysxo.html

[Q22] 排序
来源：http://hz.hongshengwenyu.top/gtmhybmqhx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhaomingkeji.xyz/gtedtbvqsa.html

[Q23] 分页
来源：http://hz.xuanzx.com/gtigzlbsii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.redwolf501.top/gtquzhwodh.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtkmawmehz.html

SELECT DISTINCT city FROM users;
来源：http://hz.yueranfly.top/gtajmnfcxn.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gtewywfnfx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hongshengwenyu.top/gtlvmrfnzu.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtpwytespv.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtlsfqhitx.html

[Q27] 条件计数
来源：http://hz.zhiwuduotai.top/gtcarpjbzd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gogol.net.cn/gtafujnyyf.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gttlrtbxzk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtgeuhqsan.html

[Q29] 最大最小值
来源：http://hz.0kj1m.cn/gtvlzzfrgr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gaohongyu789.top/gtqsncwhuj.html

[Q30] 分组统计
来源：http://hz.zhongyouzk.top/gtsspscaad.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtrqhkgjxj.html

[Q31] 分组后过滤
来源：http://hz.bjfxy.top/gtmpwjvzor.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtjnuwdwni.html

[Q32] 分组拼接字符串
来源：http://hz.hysaishi.cn/gtihzauwyx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gttrvnpnlw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daria6918.cn/gtnrbbqicd.html

[Q33] 多列分组
来源：http://hz.meibo888.top/gtrkkhptxt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gotoacloud.top/gtyskfffkr.html

[Q34] 每组取第一条
来源：http://hz.9152youxi.cn/gtmkkjbnyd.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gttzygvjdj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shzxlz.cn/gtvtscwepv.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtpggwkbbt.html

[Q35] 内连接
来源：http://hz.daxiang520.top/gtqswrroqq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtueirzesc.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtwstigvwk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tanke756.top/gtxtihtdav.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtlmqjksce.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigfzy.top/gtuzvbfoyd.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtuuftnrtb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxuanxn.top/gtdlntldhf.html

[Q39] 自连接（查上下级）
来源：http://hz.dashuyun.cn/gttodtuzom.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtkyuyqahw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtzttfmsah.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gtfkanyxgo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtryefsvdm.html

[Q41] 多表连接
来源：http://hz.jinyuanbaomall.cn/gthdwhgwpp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shangyingyoupin.top/gtdxjvekgv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.c1oappe.top/gtijqxswxi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtgkefawfe.html

[Q42] 连接条件附加过滤
来源：http://hz.andypj.xyz/gtsnjiqgwf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtecpimmoi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gtbeiczaux.html

[Q43] 标量子查询
来源：http://hz.xziqi.cn/gttinnvwyq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtyxviuyxt.html

[Q44] IN 子查询
来源：http://hz.jlsjyb.cn/gteqvfopuu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuxming.cn/gtnvmvivgm.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtxpygnglj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtnjfpuejh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhijiandao.cn/gtqhfqjucb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtlkcinzng.html

[Q47] 与平均值比较
来源：http://hz.aizwys.cn/gtksaybwee.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtrlhpmhyr.html

[Q48] CTE 公用表表达式
来源：http://hz.xinyue.icu/gtgtphegot.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtiimqzxzn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xinyue.icu/gtwzhjqzyg.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtjeqeedyx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zycfv.cn/gtnjweyhsn.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtxwurdigp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtpbnrozdb.html

[Q51] 用子查询更新
来源：http://hz.zhixingplan.top/gtazhwncgj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtmjkdfvcg.html

[Q52] 删除指定行
来源：http://hz.hammf.cn/gtecjddvuu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gtkykqdnoo.html

[Q53] 按条件删除
来源：http://hz.sysykeji.top/gtciwovxwm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guowangkeji.top/gtpzgtpdnh.html

[Q54] 清空表
来源：http://hz.yj202588.top/gtrbrvmocx.html

TRUNCATE TABLE logs;
来源：http://hz.yangfankeji.com/gtfeqvzqre.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigfzy.top/gtietwhxmz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtyqsxtplh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtqzqpfpli.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnqzz.top/gtwrvouoyf.html

[Q57] 行号
来源：http://hz.daxiang520.top/gtnunipquy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fzhhl.top/gtnwbbzwbf.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtorctecwj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtnttxbavi.html

[Q59] 分组内累计
来源：http://hz.jyoumei.cn/gtljiqrucb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigufen.top/gtjzhipaix.html

[Q60] 取上一行 / 下一行
来源：http://hz.gotoacloud.top/gttwgemlej.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtslxpccmv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinghuilouyu.cn/gtjbdrxmdw.html

[Q61] 移动平均
来源：http://hz.pengpengdd.cyou/gtpvdxwnxf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yvedp.cn/gtkatotlmf.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtufwklrut.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtjfavaeqa.html

[Q63] 开启事务
来源：http://hz.ydjk.org.cn/gttidzvysh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtbcbdeecb.html

[Q64] 提交事务
来源：http://hz.hongshengwenyu.top/gtiutfiscc.html

COMMIT;
来源：http://hz.jqgfzy.top/gtqgvnrpqs.html

[Q65] 回滚事务
来源：http://hz.hfpthk.cn/gtzkbliyye.html

ROLLBACK;
来源：http://hz.xinyue.icu/gtrfyhyvqp.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtjjudajer.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258.top/gteqklenqg.html

[Q67] 设置隔离级别
来源：http://hz.ivvv.top/gtateatclv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gtpfowdymt.html

[Q68] 保存点
来源：http://hz.mhx1999.top/gtikxclwzy.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtbvaizkag.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtselcnjph.html

[Q69] 查看执行计划
来源：http://hz.andypj.xyz/gttlabpddl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ybcxt.top/gtqbmjrbei.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtjvihvywy.html

ANALYZE TABLE users;
来源：http://hz.dashuyun.cn/gtonwzuffd.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtglfdmcey.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gthbpdifzr.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtffhxxvun.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gtlzqjdlov.html

[Q73] 查看表状态
来源：http://hz.birdmap.top/gtvlervcac.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yvedp.cn/gtlzexfufd.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gtfrqhldjj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtkmttvqml.html

[Q75] 日期格式化
来源：http://hz.zycfv.cn/gtdgnaomme.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.316326.xyz/gtmmojsdvj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtuchkxczx.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtbtsrzevd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtjtnvenqz.html

[Q77] 时间加减
来源：http://hz.jinqigfzy.top/gtmxzjihuf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtfoeuksfb.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtivagyxxv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ivvv.top/gtgtwierid.html

[Q79] 字符串拼接
来源：http://hz.cheryme.top/gtdpkqmhkr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.smart0.xyz/gtduedowzp.html

[Q80] 字符串截取
来源：http://hz.guannengcc.top/gtlraqwixj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gtfckoshmq.html

[Q81] 字符串替换
来源：http://hz.9152youxi.cn/gtunxbqhpo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zycfv.cn/gtfhkuttze.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtdganxhwd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtgcpykthu.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtkjexfzyn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtdpjgyjlz.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtyzzbywnl.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtjxplbrxp.html

[Q85] 数值取整
来源：http://hz.zhongyouzk.top/gtieaxoobr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtvyyzyqwx.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtzaeaiqdi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtupnkdwfb.html

[Q87] JSON 字段做条件
来源：http://hz.jinyuanbaomall.cn/gtbumrbseq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ywan-chungtsiang.top/gthyjjsimo.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinghuilouyu.cn/gtihgtsliu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gtzpvqznfr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtabqwlyde.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtasczwpow.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gthwlugkml.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gtmwuqijjx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtgofsidut.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtiyzcepdt.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gtsuldeyfv.html

================================================================================
来源：http://hz.aizwys.cn/gtgmxrsxxs.html

[R01] shebang 与严格模式
来源：http://hz.jlsjyb.cn/gtweqgvezk.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtjwzzcrin.html

set -euo pipefail
来源：http://hz.shanyushiyangtech.top/gtczeoiktg.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtydevgkrg.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtcknvtjcc.html

[R03] 只读变量
来源：http://hz.tian-w.cn/gtxcxwuzla.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtxsuylrwo.html

[R04] 位置参数
来源：http://hz.xylfe.cn/gtgnhmiusj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gthwxhcsep.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtcsckyvnc.html

name="${1:-default}"
来源：http://hz.yj20258888.top/gtcgehjvsr.html

[R06] 判断命令是否存在
来源：http://hz.fengsongda.top/gteyjmyjjq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gaohongyu789.top/gtqxmtsjnu.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtxmypnpyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtphhdtyur.html

[R08] 数值比较
来源：http://hz.hammf.cn/gtgqtffnfp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtoemblbpw.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtftfyfatn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtkoijfewv.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtcoatixqp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jlsjyb.cn/gtwjytjuad.html

[R11] case 多分支
来源：http://hz.hysaishi.cn/gtpiehjorh.html

case "$1" in
来源：http://hz.havefunace.top/gtomzacuxv.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtlibntitn.html

stop)  echo "停止" ;;
来源：http://hz.yj20258.top/gtjeowaigq.html

*)     echo "未知命令" ;;
来源：http://hz.cucudq.cn/gtlnbedfmv.html

esac
来源：http://hz.ywan-chungtsiang.top/gtmwqkbzak.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtpjwsbten.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shuidangran.top/gtwupyhibi.html

[R13] for 计数循环
来源：http://hz.hywenlv.cn/gtikifwzaa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtrkcravpq.html

[R14] C 风格 for
来源：http://hz.haohaochexian.top/gthsvswhxt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenjidiqi.icu/gtniberrlx.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtvuezyvkz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtsolgkgte.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtlzlsazlv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtokxkelky.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtstecfapb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yueranfly.top/gtvmomidts.html

[R18] 遍历数组
来源：http://hz.ivvv.top/gtdstxwlbz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenjidiqi.icu/gtudoqfjmx.html

[R19] 数组长度
来源：http://hz.yangfankeji.com/gtzyonnjwa.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gttmjflris.html

[R20] 关联数组（字典）
来源：http://hz.zhongyouzk.top/gthlcpcikt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhijiandao.cn/gtgomdsehs.html

[R21] 字符串长度
来源：http://hz.aibaodan.cn/gtrqxhxlug.html

echo "${#s}"
来源：http://hz.chenjidiqi.icu/gtsjenndrf.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtbeqebwbn.html

echo "${s:0:5}"
来源：http://hz.vqdsnc.cn/gtqymsrhlm.html

[R23] 字符串替换
来源：http://hz.nwbrower.top/gtcqaejdiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtlnppnhgt.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtziroqsyd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ehwqpu.com/gtcmfpqwpq.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxuanxn.top/gtawzzlfni.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtietzxrpr.html

[R26] 命令替换
来源：http://hz.yongpay.top/gtsgwkrhyk.html

now=$(date +%F); echo "$now"
来源：http://hz.chenjidiqi.icu/gtmotreppw.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtwvalcxfq.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258.top/gthesfgodl.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtkmmiyasu.html

echo "scale=2; 10/3" | bc
来源：http://hz.yvedp.cn/gtovhodyqo.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtdodzqzfn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtkbkvtfdr.html

[R30] 函数返回状态码
来源：http://hz.mhx1999.top/gtaqaxoefz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigufen.top/gtydtbjtzk.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtynnjyssw.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtmsanzhkj.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gttfvwnxyc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtrectsmnf.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtdzgpgcnd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtqevfqsdt.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtblvepocf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtvpjwazfo.html

[R35] 后台执行并等待
来源：http://hz.gaohongyu789.top/gtxjwrfrey.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtzbfmxdxo.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtqcnfzzgy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtotfppdup.html

[R37] 把输出赋给变量
来源：http://hz.svipenyu.cn/gtvxcolisd.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtsenmhcfz.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtdvuhtchd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.kuanghao11.cn/gtruzwfbti.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gtlqsyfhfz.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gtvsrngljt.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gtcghegmew.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gtsflvezvn.html

[R41] 丢弃输出
来源：http://hz.tian-w.cn/gtvclyleck.html

cmd >/dev/null 2>&1
来源：http://hz.jyoumei.cn/gtjjyqnqdc.html

[R42] 输入重定向
来源：http://hz.aibaodan.cn/gtlwgkainb.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtdcyfdpci.html

[R43] 按名字查找文件
来源：http://hz.jlsjyb.cn/gtchmnwdes.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtrneuiawc.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtngrxvwqp.html

find . -mtime -7 -type f
来源：http://hz.shuidangran.top/gtfsylhakj.html

[R45] 批量删除
来源：http://hz.shanyushiyangkeji.top/gtchnivbsa.html

find . -name "*.tmp" -delete
来源：http://hz.vqdsnc.cn/gtcmgtannw.html

[R46] 递归替换文件内容
来源：http://hz.xziqi.cn/gtuxxhokwy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtqrlxpryg.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtudhjplma.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cheryme.top/gtslghrjhn.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtxxufpkjz.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtcgwlwzgb.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtgjqfngta.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinqigufen.top/gtsirmblpv.html

[R50] awk 求和
来源：http://hz.yanxiufei.cn/gtfrydektm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtarphcajt.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtvnaznljs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtsdqwnuel.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtozmypkkm.html

wc -l a.txt
来源：http://hz.zhongyouzk.top/gtpqwhwwrm.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtsklhuxna.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenlongwang.top/gtubjyimcb.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtndjoecgw.html

diff a.txt b.txt
来源：http://hz.xziqi.cn/gtnatuvaes.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtrcaskcbt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gotoacloud.top/gthkjqemcr.html

[R56] 远程拷贝
来源：http://hz.tianlin.xyz/gtsahojyeg.html

scp file user@host:/path/
来源：http://hz.ehwqpu.com/gtxrvqxxep.html

[R57] 远程执行命令
来源：http://hz.hywenlv.cn/gtijuonilo.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gtnjartiwz.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtnflosgli.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtitffesat.html

[R59] 发 POST JSON
来源：http://hz.yongpay.top/gtghmkkvfx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtceedfouk.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258.top/gtezdnnhen.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtfvylmqxp.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gthqjckvsl.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtmuzqvnej.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtgufmfujl.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtjtjgsyey.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtvqvysehi.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gtdsctaojy.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtiwtpzxuc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtwpibotyb.html

[R65] 查看端口占用
来源：http://hz.snrcjt.cn/gtygxsfihy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shangyingyoupin.top/gtxymlcwxe.html

[R66] 定时任务
来源：http://hz.cqqwz.cn/gthwnlbrgu.html

crontab -e;  crontab -l
来源：http://hz.xingfuxueyuan.xyz/gtvkoprigu.html

[R67] 生成随机十六进制串
来源：http://hz.wangshuangyany.cn/gtlkutewuy.html

openssl rand -hex 16
来源：http://hz.zhongyouzk.top/gtkkyplhje.html

[R68] 计算文件校验值
来源：http://hz.c1oappe.top/gtvqqfypgs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtvnvaslbq.html

[R69] 生成随机密码
来源：http://hz.jinyuanbaomall.cn/gtibdlbrwu.html


<!-- 参考信息 -->