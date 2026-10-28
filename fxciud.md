代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gtjixgqcsh.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtvtlosgtg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhijiandao.cn/gtqbitcawj.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtzgkbggnk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gtakrammfb.html

[Q24] 去重
来源：http://hz.tian-w.cn/gtnqaqjgtq.html

SELECT DISTINCT city FROM users;
来源：http://hz.redwolf501.top/gtupovwqya.html

[Q25] 只取前 N 条
来源：http://hz.pengpengdd.cyou/gturqhjmnt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aibaodan.cn/gtbosdozgk.html

[Q26] 计数
来源：http://hz.316326.xyz/gtinfehclt.html

SELECT COUNT(*) FROM users;
来源：http://hz.feifeiyinyue.top/gtfobdsppu.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gttnmujznm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.quarkkingdee.top/gtidvhgzsi.html

[Q28] 求和与平均
来源：http://hz.feifeiyinyue.top/gtofuyamln.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hywenlv.cn/gttwvhlhml.html

[Q29] 最大最小值
来源：http://hz.dianchejie.cn/gtpjardtvz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtjntwlskf.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtebehyjik.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtkpbaoaxq.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gticasaonu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.snrcjt.cn/gtdkgxaoli.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtklswkiyy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gthtprbfkw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtbkoljlfv.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtgbrpnfuz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shuidangran.top/gtyapqqijt.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtmkinfopi.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtdtvulbjr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.316326.xyz/gtsqzeuvgt.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtpfhvfdwn.html

[Q35] 内连接
来源：http://hz.c1oappe.top/gtgvfgzvkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtenygeszl.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gthkvokfrt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtfagetcjb.html

[Q37] 右连接
来源：http://hz.shanyushiyangtech.top/gtrgsxcsyo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yanxiufei.cn/gtdwecouoe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtzullprwz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenzaomai.com/gtwfhgijxm.html

[Q39] 自连接（查上下级）
来源：http://hz.cqqwz.cn/gtbamzcyci.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.mhx1999.top/gtzvfshjbe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtkkrfblxv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtgdvodxmb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.snrcjt.cn/gtknzrwvft.html

[Q41] 多表连接
来源：http://hz.ydjk.org.cn/gtnpopgryi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gzhubu.top/gtvzujwpxa.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtyagqhaus.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtsatjmkst.html

[Q42] 连接条件附加过滤
来源：http://hz.zhixingplan.top/gtsunzcwih.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtgpuctmxf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtsnuuyicj.html

[Q43] 标量子查询
来源：http://hz.yueranfly.top/gtixctlpej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gtoodpvqkd.html

[Q44] IN 子查询
来源：http://hz.hnqzz.top/gtboxlnjtm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhiwuduotai.top/gtuifxlgfj.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtvkizjxfj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtqhdefxwn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtcmtpxngr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xingfuxueyuan.xyz/gtozqtlpfk.html

[Q47] 与平均值比较
来源：http://hz.hysaishi.cn/gtscwvcoun.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fengsongda.top/gtuevwjnnn.html

[Q48] CTE 公用表表达式
来源：http://hz.tian-w.cn/gtdbbhoizd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtyjbdxtap.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtsibmubdr.html

[Q49] 更新单行
来源：http://hz.meibo888.top/gtdeahxllp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gthonqxhzp.html

[Q50] 批量更新
来源：http://hz.xuetiantiany.cn/gtusdxakqg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gtugpfromm.html

[Q51] 用子查询更新
来源：http://hz.jqgufenzy.top/gtbvmxlrfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhiwuduotai.top/gtqnhplrka.html

[Q52] 删除指定行
来源：http://hz.wangshuangyany.cn/gtmjnguwfp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtwcrxjccn.html

[Q53] 按条件删除
来源：http://hz.jqgfzy.top/gthkgczoed.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtepwnaoqn.html

[Q54] 清空表
来源：http://hz.yanxiufei.cn/gtfmdowccr.html

TRUNCATE TABLE logs;
来源：http://hz.316326.xyz/gthyqhsely.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtlotcesjr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtaptmswmi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cashguo.top/gtmtuxjzpu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenjidiqi.icu/gtuvkftbjm.html

[Q57] 行号
来源：http://hz.pycfn.com/gtbketsosg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtaegeryyi.html

[Q58] 累计求和
来源：http://hz.cqqwz.cn/gtrolkznwf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.birdmap.top/gtkhbgzjgs.html

[Q59] 分组内累计
来源：http://hz.jinqigfzy.top/gtebycjudd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gotoacloud.top/gtjksrqnys.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtftmypain.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hfpthk.cn/gtasfggcgj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtdefizaoa.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gthvvwetwk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtlxrmgpro.html

[Q62] 分组占比
来源：http://hz.chenjidiqi.icu/gtfixqqtww.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gteamarlhr.html

[Q63] 开启事务
来源：http://hz.jinqigufen.top/gtscztlsnh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sxryk.cn/gthygexmja.html

[Q64] 提交事务
来源：http://hz.svipenyu.cn/gtswhdxdnw.html

COMMIT;
来源：http://hz.c1oappe.top/gtvpdnvevf.html

[Q65] 回滚事务
来源：http://hz.tianlin.xyz/gtgxznqcxz.html

ROLLBACK;
来源：http://hz.shzxlz.cn/gtfjqaprmm.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gtpmfaahzc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtmvyzcpeh.html

[Q67] 设置隔离级别
来源：http://hz.jinqigfzy.top/gtdscjthvi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gterliaohh.html

[Q68] 保存点
来源：http://hz.nwbrower.top/gttffukekm.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtnljdform.html

ROLLBACK TO sp1;
来源：http://hz.hfpthk.cn/gtcngrjlgx.html

[Q69] 查看执行计划
来源：http://hz.jinqigfzy.top/gtovyjcfts.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtmbilttjy.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtlnmhutbg.html

ANALYZE TABLE users;
来源：http://hz.ehwqpu.com/gtjmkbnycd.html

[Q71] 查看建表语句
来源：http://hz.jyoumei.cn/gtjmglvzjo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtcrfmhpoy.html

[Q72] 查看索引
来源：http://hz.cheryme.top/gtdoleoaqc.html

SHOW INDEX FROM users;
来源：http://hz.zhengqikj.top/gtvfucvnon.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gtvbebsngp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yueranfly.top/gtiqlsbcco.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtsneodkql.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtxbgbqvco.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gttmnepyqo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtxawqmnou.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gttwbqwjna.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtxsgzwtyo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yj20258888.top/gtuacfhxqv.html

[Q77] 时间加减
来源：http://hz.birdmap.top/gtkbnuxvbt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gtyohdaiuf.html

[Q78] 当前时间
来源：http://hz.guannengcc.top/gtgylnjvjm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aibaodan.cn/gtzhidynpv.html

[Q79] 字符串拼接
来源：http://hz.jyoumei.cn/gtbiuedqfp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hywenlv.cn/gtpqeaoctm.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtwakiefqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hywenlv.cn/gtfoijorjb.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gttasmwlnq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtclerwylv.html

[Q82] 字符长度与字节长度
来源：http://hz.aizwys.cn/gtwhhwmbhf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtqeetaywy.html

[Q83] 大小写转换
来源：http://hz.0kj1m.cn/gtrrfqgojp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtqbpqocii.html

[Q84] 去除首尾空格
来源：http://hz.hfpthk.cn/gtdnazwhlz.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtglknzvxn.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gtseubyjwt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtfvzgrftx.html

[Q86] 读取 JSON 字段
来源：http://hz.daria6918.cn/gtbjstbyge.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jyoumei.cn/gtzkfefpxt.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtwwlvfhcv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hongshengwenyu.top/gthqjbasca.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtyytueizh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xingfuxueyuan.xyz/gtsrttllev.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yueranfly.top/gtacnemtpm.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtrfthvjov.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xylfe.cn/gtoirgvzsc.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtiblpiouz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtpfhrfkmv.html

================================================================================
来源：http://hz.yongpay.top/gtlhctbztw.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gtbwnftyoe.html

================================================================================
来源：http://hz.ybcxt.top/gtzleplkca.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtbajvvpzv.html

#!/usr/bin/env bash
来源：http://hz.birdmap.top/gtteprgwks.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtlvdxdrjn.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtrezycxnu.html

name="Tom"; echo "$name"
来源：http://hz.jlsjyb.cn/gtmfwuhieo.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtnvamoozk.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gthrnherfz.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtzyfdwfpn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aibaodan.cn/gtohodmnsg.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtjpivqtlo.html

name="${1:-default}"
来源：http://hz.jqgfzy.top/gtlrvvmqjz.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gthlmkqfxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtjcuoixpx.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtmbkmzmms.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.feifeiyinyue.top/gtixwrkgls.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gttuzihamh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hfpthk.cn/gtqkemxsdq.html

[R09] 字符串比较
来源：http://hz.cheryme.top/gtrifdrfgq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jiagoushi.top/gtyznrvrtu.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gtbpdlfplb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnqzz.top/gthpnzxcnd.html

[R11] case 多分支
来源：http://hz.cucudq.cn/gtuugtyhgw.html

case "$1" in
来源：http://hz.haohaochexian.top/gtgjcjxzsz.html

start) echo "启动" ;;
来源：http://hz.daria6918.cn/gtjprjhnsn.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtamfegodc.html

*)     echo "未知命令" ;;
来源：http://hz.sysykeji.top/gtxueldcrg.html

esac
来源：http://hz.wangshuangyany.cn/gtylqtncnz.html

[R12] for 遍历文件
来源：http://hz.guowangkeji.top/gtvsxfivsf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.svipenyu.cn/gtnamsiqyq.html

[R13] for 计数循环
来源：http://hz.ydzc1.top/gtigtycgza.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtlhbbkzyq.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtdssjmjpu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtjpffbyeg.html

[R15] while 逐行读文件
来源：http://hz.vqdsnc.cn/gtxtpioewk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhongyouzk.top/gtoxascwie.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtghgmudkf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtkedhgdtm.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtkiqvgqxq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhongyouzk.top/gtkvbpbtgp.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtdqfqbkkv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtetxdmrlq.html

[R19] 数组长度
来源：http://hz.cqqwz.cn/gtwwgmgfks.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtqficxupi.html

[R20] 关联数组（字典）
来源：http://hz.havefunace.top/gtmxvgkvof.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gtrclbaivd.html

[R21] 字符串长度
来源：http://hz.sufxvd.cn/gtfilykzcm.html

echo "${#s}"
来源：http://hz.52xcode.cn/gtdssfcsib.html

[R22] 截取子串
来源：http://hz.zhixingplan.top/gtjeppmlsh.html

echo "${s:0:5}"
来源：http://hz.zhiwuduotai.top/gtluescyed.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtqsgrvtac.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jianghu66.top/gtqsuwtteq.html

[R24] 大小写转换
来源：http://hz.yvedp.cn/gtnwzudjyk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtypxrpjmi.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtmctkglty.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuanzx.com/gtddhacyau.html

[R26] 命令替换
来源：http://hz.cucudq.cn/gtogeunwna.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtprqnsevt.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtfmkqvdjl.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtwsnhthew.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtnnritgta.html

echo "scale=2; 10/3" | bc
来源：http://hz.xziqi.cn/gtedjcytpg.html

[R29] 定义函数
来源：http://hz.cucudq.cn/gtsfkmouqo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gtbsjykzeb.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtklxxcfax.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtudyhogdd.html

[R31] 局部变量
来源：http://hz.vqdsnc.cn/gtiyqwdnao.html

f() { local x=1; echo "$x"; }
来源：http://hz.jianghu66.top/gtlkknfymk.html

[R32] 参数个数校验
来源：http://hz.snrcjt.cn/gtjpuzggeo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gtdjvbwksi.html

[R33] 捕获错误并提示行号
来源：http://hz.yanxiufei.cn/gtvhindwee.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtibjqrrkg.html

[R34] 退出时清理
来源：http://hz.nwbrower.top/gthsondbvt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtsbwzmbif.html

[R35] 后台执行并等待
来源：http://hz.9152youxi.cn/gtrvhftjax.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ehwqpu.com/gtjserhefa.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gtdasjfvik.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtpuzwfjiv.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtoqivvmqt.html

files=$(ls -1)
来源：http://hz.jlsjyb.cn/gtpicmizfz.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtnceiwdef.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gtqkbdlfgf.html

[R39] 重定向标准输出与错误
来源：http://hz.9152youxi.cn/gtxmapoaov.html

cmd > out.log 2>&1
来源：http://hz.nanxinkj.top/gtmxntujom.html

[R40] 追加写日志
来源：http://hz.yuxming.cn/gtxyhkhjld.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtpyqsfind.html

[R41] 丢弃输出
来源：http://hz.svipenyu.cn/gtwjcjcdzh.html

cmd >/dev/null 2>&1
来源：http://hz.bjfxy.top/gtatosijua.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gtkaykkbtp.html

wc -l < a.txt
来源：http://hz.daria6918.cn/gtqykklwum.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtsyzzsmvc.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtbujznssb.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtadssfwms.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gtkvlobrlt.html

[R45] 批量删除
来源：http://hz.pengpengdd.cyou/gtbopmwtlx.html

find . -name "*.tmp" -delete
来源：http://hz.0kj1m.cn/gtwfddwucb.html

[R46] 递归替换文件内容
来源：http://hz.shzxlz.cn/gtvvdwwrbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgfzy.top/gthzxoobia.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtfqcvwmvw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtombyqres.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtbrhwjacx.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtvbjkifzj.html

[R49] awk 带条件
来源：http://hz.jinqigfzy.top/gtassamyco.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangkeji.top/gtrmzvhhyi.html

[R50] awk 求和
来源：http://hz.xingfuxueyuan.xyz/gtugnauuku.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtqeazgekx.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtmfgesntr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gttbfjpuld.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtmhpbufqk.html

wc -l a.txt
来源：http://hz.meibo888.top/gtbhovxwvc.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtivqdadth.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtpgehgesr.html

[R54] 比较两个文件
来源：http://hz.jinqigufen.top/gtxmhktiow.html

diff a.txt b.txt
来源：http://hz.yueranfly.top/gtylbtodsg.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtjdsdbceg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.birdmap.top/gtewfhrrkj.html

[R56] 远程拷贝
来源：http://hz.yonumen.top/gtwefbdzne.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtwvpehrvm.html

[R57] 远程执行命令
来源：http://hz.gaohongyu789.top/gtnyckdzaq.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtwyjnjywf.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gtriajexze.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gteoojyyzb.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gttqqbudfk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jiagoushi.top/gtxurcgqdy.html

[R60] 只看 HTTP 状态码
来源：http://hz.sweek.top/gtkxkypbop.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtqvxttdtf.html

[R61] 磁盘占用
来源：http://hz.cqqwz.cn/gtlsljuhdh.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtfvmvhpwr.html

[R62] 找最占空间的文件
来源：http://hz.gotoacloud.top/gtxqejluoz.html

du -ah . | sort -rh | head -10
来源：http://hz.daria6918.cn/gtldqwhizu.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtfprruldt.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtfucqzlbl.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtkypsajao.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258888.top/gthnbcvrtv.html

[R65] 查看端口占用
来源：http://hz.shzxlz.cn/gtpqzerzvz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.vqdsnc.cn/gtlfzjjkmh.html

[R66] 定时任务
来源：http://hz.52xcode.cn/gtmzjonnfh.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtjvpmnllj.html

[R67] 生成随机十六进制串
来源：http://hz.zhongyouzk.top/gtnnfdkcvq.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtvvuimgcm.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gtizrxgknw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtwdjnoyft.html

[R69] 生成随机密码
来源：http://hz.ivvv.top/gtkfcbozhm.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtbcnpyjfi.html

[R70] 时间戳与互转
来源：http://hz.zhiwuduotai.top/gtzwznsxtf.html

date +%s;  date -d @1700000000
来源：http://hz.bjfxy.top/gtzeslinxy.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gthbzwdksg.html


<!-- 参考信息 -->