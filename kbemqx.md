代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pycfn.com/gtkyeiqrmx.html

[Q24] 去重
来源：http://hz.sxryk.cn/gtfpbfydfn.html

SELECT DISTINCT city FROM users;
来源：http://hz.yanxiufei.cn/gtljyuwhiz.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtvyimdfqk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinghuilouyu.cn/gtidgvcple.html

[Q26] 计数
来源：http://hz.shanyushiyangtech.top/gtatrxbnag.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtlfhmuypb.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtlamfcbvw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.kuanghao11.cn/gtkyqsebnb.html

[Q28] 求和与平均
来源：http://hz.xingfuxueyuan.xyz/gtukuvjhjx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jiagoushi.top/gtlluwirci.html

[Q29] 最大最小值
来源：http://hz.fengsongda.top/gtpcvhjirc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtqjizbgzs.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtoecgmxkr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gttqosgonb.html

[Q31] 分组后过滤
来源：http://hz.wangshuangyany.cn/gtncxkbrcz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sufxvd.cn/gtjuhsfeau.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtcyykytty.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtmqinsbud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.c1oappe.top/gtawtitwsn.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gthfmdhezb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sxryk.cn/gtwvmvwioe.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtztwyfefw.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtguvalgwp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dianchejie.cn/gthqatbgdf.html

) t WHERE rn = 1;
来源：http://hz.gzhubu.top/gtrgjlydau.html

[Q35] 内连接
来源：http://hz.zhengqikj.top/gtmawwriff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtchlsacxx.html

[Q36] 左连接
来源：http://hz.xingfuxueyuan.xyz/gtjhkyotzv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtzkwvihus.html

[Q37] 右连接
来源：http://hz.hnxiangtu.top/gtwxoyxgxk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gtqwgxavbx.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtqgehquzn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtlmdaykiz.html

[Q39] 自连接（查上下级）
来源：http://hz.cheryme.top/gtwnhhtugl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtnqvebaax.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gtrposjkvy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zdqjudy.top/gticokzluz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtrzijcwin.html

[Q41] 多表连接
来源：http://hz.chenzaomai.com/gtktjfohwp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cucudq.cn/gtoigabezh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtiqvekxrd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guowangkeji.top/gtqplbxvkp.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtxopdwkic.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhoulong.xyz/gtwtufucdh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtcxvwkrbn.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtcymcsubs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zdqjudy.top/gtsskfibhm.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtuocakzkl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gteynpehho.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtvgxmrdfu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtrgansneu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhixingplan.top/gtxnsqdpkn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtkqspgimk.html

[Q47] 与平均值比较
来源：http://hz.yuanzhike.top/gtkrrsaxer.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sufxvd.cn/gtciwaajwq.html

[Q48] CTE 公用表表达式
来源：http://hz.cdnleiting.top/gthmhajoci.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tianlin.xyz/gtaepdyfzr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ywan-chungtsiang.top/gtedsafqur.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gtjckonnzr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtxokmvwqh.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtndrzcxkc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ppjwa.cn/gtszhpmskk.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtgompsykf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtonktfxaj.html

[Q52] 删除指定行
来源：http://hz.bjfxy.top/gtglammayk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gtoufmqfqv.html

[Q53] 按条件删除
来源：http://hz.aibaodan.cn/gttzsnakjc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.52xcode.cn/gtujklsxgu.html

[Q54] 清空表
来源：http://hz.zhoulong.xyz/gtdrkslydd.html

TRUNCATE TABLE logs;
来源：http://hz.jlsjyb.cn/gtiiijgswo.html

[Q55] 排名（并列占位）
来源：http://hz.guannengcc.top/gtugjwdzqq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.meibo888.top/gtchwhhikn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydjk.org.cn/gtdtsvbany.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtwzktyztr.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtjywwnvpm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zdqjudy.top/gtfthgralg.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtzpugfvyv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtaqaylflj.html

[Q59] 分组内累计
来源：http://hz.hongshengwenyu.top/gtatwuucll.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gtzoamowsa.html

[Q60] 取上一行 / 下一行
来源：http://hz.cucudq.cn/gtqbkayztb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtqvrgzyfq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xziqi.cn/gtxhhvdbku.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gthjjaxpiq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nwbrower.top/gtxikhvcay.html

[Q62] 分组占比
来源：http://hz.hongshengwenyu.top/gtvofefuxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtywphnkod.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gtvyzebwrz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yanxiufei.cn/gtcqluwgen.html

[Q64] 提交事务
来源：http://hz.ydjk.org.cn/gthgicytvg.html

COMMIT;
来源：http://hz.hywenlv.cn/gtjharouov.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtoutrixzb.html

ROLLBACK;
来源：http://hz.jinqigufen.top/gtaaiqclos.html

[Q66] 行锁查询
来源：http://hz.tian-w.cn/gtshsgcred.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.dashuyun.cn/gtxqhitzpe.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtikzrdjgx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtpbwbbcvh.html

[Q68] 保存点
来源：http://hz.gotoacloud.top/gtbkrummxk.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtqsncsofb.html

ROLLBACK TO sp1;
来源：http://hz.zhaomingkeji.xyz/gtpvrioraf.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtqmslxzji.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cashguo.top/gtnkzalqtt.html

[Q70] 更新统计信息
来源：http://hz.daxiang520.top/gttvzzxxoq.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtconiemyi.html

[Q71] 查看建表语句
来源：http://hz.jianghu66.top/gtsrlxbzkv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydzc1.top/gtvkvwcclj.html

[Q72] 查看索引
来源：http://hz.jyoumei.cn/gtwpdrffdd.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtztgivzhh.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtedyyjqau.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gtktiedvep.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gthnohkmxt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtbwfrhwpl.html

[Q75] 日期格式化
来源：http://hz.9152youxi.cn/gtmnqsiwli.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtvhmpkldn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.wangshuangyany.cn/gtitolwbwz.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gttwwnmlpa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxuanxn.top/gtbktxvall.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtaytjxrrk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hfpthk.cn/gtanlihmvr.html

[Q78] 当前时间
来源：http://hz.snrcjt.cn/gtgsghffxu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.svipenyu.cn/gtfmxtgvia.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtvvrywkbi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daria6918.cn/gtngfbffin.html

[Q80] 字符串截取
来源：http://hz.tian-w.cn/gtbcshgire.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtksukpsmr.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtcgoobhlh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtxoochlfq.html

[Q82] 字符长度与字节长度
来源：http://hz.bjfxy.top/gttpcqnuln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gttgjfyegi.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtjnksdagf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtvbuqaxln.html

[Q84] 去除首尾空格
来源：http://hz.bjfxy.top/gtplswasvh.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtpkpagifq.html

[Q85] 数值取整
来源：http://hz.snrcjt.cn/gtixmalenh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ehwqpu.com/gttfaqqndy.html

[Q86] 读取 JSON 字段
来源：http://hz.hnqzz.top/gtlwzchhqk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gttpagqsxe.html

[Q87] JSON 字段做条件
来源：http://hz.zhongyouzk.top/gtdoasjssx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangtech.top/gtitmehudb.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangkeji.top/gtxucnjoob.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtjgeainhx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtjbhwhais.html

[Q89] 判断表是否存在
来源：http://hz.tian-w.cn/gtpwtsegtc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daria6918.cn/gtvgrktcax.html

[Q90] 生成序号列
来源：http://hz.yvedp.cn/gtbjcaomub.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtmmunzrkj.html

================================================================================
来源：http://hz.shuidangran.top/gtwtvvdsts.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gttacdnjhj.html

================================================================================
来源：http://hz.cucudq.cn/gtkvcoxlru.html

[R01] shebang 与严格模式
来源：http://hz.sufxvd.cn/gtgdxddgns.html

#!/usr/bin/env bash
来源：http://hz.cheryme.top/gticiusfuy.html

set -euo pipefail
来源：http://hz.zdqjudy.top/gtetgcsvrt.html

[R02] 变量赋值与使用
来源：http://hz.yangfankeji.com/gtqlyyawok.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtxbkkvygx.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtvbhdmmko.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtyvflqvdz.html

[R04] 位置参数
来源：http://hz.vqdsnc.cn/gtxfmoqrzi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangkeji.top/gtdosqzmyd.html

[R05] 参数默认值
来源：http://hz.shuidangran.top/gtkauwdanj.html

name="${1:-default}"
来源：http://hz.xziqi.cn/gtanvwqqwa.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtrskiwgwc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.havefunace.top/gthwoizeco.html

[R07] if 判断文件
来源：http://hz.jiagoushi.top/gtrzsutjud.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yangfankeji.com/gtzzkaqcqz.html

[R08] 数值比较
来源：http://hz.wangdashe.top/gtvdmuloph.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.316326.xyz/gtmannwwib.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtmmrhlfmd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gtzomyurmv.html

[R10] 正则匹配
来源：http://hz.sweek.top/gtiqcswghc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gtitebqtng.html

[R11] case 多分支
来源：http://hz.shzxlz.cn/gtuqiwunbc.html

case "$1" in
来源：http://hz.nwbrower.top/gttoozyctv.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangkeji.top/gtjqngmfbx.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtjdjjmzlj.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtygaffjmf.html

esac
来源：http://hz.cdnleiting.top/gteaulwgcr.html

[R12] for 遍历文件
来源：http://hz.dianchejie.cn/gtbfbcvnqn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtxrolpfkj.html

[R13] for 计数循环
来源：http://hz.quarkkingdee.top/gtfjyaurtj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhengqikj.top/gtugcrvlgj.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gtmzqdqnzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gotoacloud.top/gtdzzoipss.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gthhepdyro.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jianghu66.top/gttuegdnfg.html

[R16] until 等待条件
来源：http://hz.zhongyouzk.top/gtbfpzrkbm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gtigprmkey.html

[R17] 数组定义与取值
来源：http://hz.ydjk.org.cn/gtgplxsjgz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gttunzaznk.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gthugipoui.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtibollnuw.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtfmpynhft.html

echo "${#arr[@]}"
来源：http://hz.jinghuilouyu.cn/gtnepcrapb.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtlhoezkep.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtdxmzpcgt.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtulweyyci.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gtagtlctgn.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtzruseykl.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtttafvyup.html

[R23] 字符串替换
来源：http://hz.316326.xyz/gthrgmaghd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnqzz.top/gtdxpbsocq.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gthepswbcl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuetiantiany.cn/gtebpbptim.html

[R25] 去后缀 / 去前缀
来源：http://hz.cqqwz.cn/gtcjjqjrcs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gthzuistqv.html

[R26] 命令替换
来源：http://hz.gogol.net.cn/gtkdmsconl.html

now=$(date +%F); echo "$now"
来源：http://hz.gotoacloud.top/gteruqbffe.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtqwvmxyol.html

echo $((1 + 2 * 3))
来源：http://hz.yvedp.cn/gtscdsnduk.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gtcscqucvz.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtmdhtpypn.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtjvnwufyz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtffnqwyqq.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtpfqsgyty.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gtbffvdnxn.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtgyfzirlm.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gthenotjvo.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtenfsfoou.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtgmyddpix.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtedqlyusd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtgzzeljpz.html

[R34] 退出时清理
来源：http://hz.cqqwz.cn/gtcevaogqp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtcqiizwar.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtldughbqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gtyxgeznit.html

[R36] 并发执行多个任务
来源：http://hz.daxiang520.top/gteccdnehu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtrwuyzchl.html

[R37] 把输出赋给变量
来源：http://hz.haohaochexian.top/gtxnkbmslh.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gtnohgukzh.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtmqvivgvu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxinkj.top/gtmplxupus.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtetklkahz.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtzuaicsze.html

[R40] 追加写日志
来源：http://hz.gogol.net.cn/gtpzbudnnu.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtcmngjspn.html

[R41] 丢弃输出
来源：http://hz.0kj1m.cn/gtcftgfyfa.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtenrnzdbw.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gthbsuwjtm.html

wc -l < a.txt
来源：http://hz.daria6918.cn/gtlrccsbby.html

[R43] 按名字查找文件
来源：http://hz.feifeiyinyue.top/gthvaghwcn.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtzjbjxfth.html

[R44] 按修改时间查找
来源：http://hz.cdnleiting.top/gteukumbkq.html

find . -mtime -7 -type f
来源：http://hz.xuetiantiany.cn/gtmiapjivx.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtdgpxymsj.html

find . -name "*.tmp" -delete
来源：http://hz.fengsongda.top/gtmwpgkkyk.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtgvxhdqyc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtlixofnrm.html

[R47] sed 单行替换
来源：http://hz.hfpthk.cn/gtqqlczqzp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtcdzyuisq.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtqvwcaili.html

awk '{print $1, $3}' a.txt
来源：http://hz.iojbl.cn/gtwqywdaam.html

[R49] awk 带条件
来源：http://hz.jinyuanbaomall.cn/gtsllaggin.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtuucaeuzw.html

[R50] awk 求和
来源：http://hz.zhiwuduotai.top/gtpoiypwsb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yuanzhike.top/gtryftzfqn.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtpoiacdbv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuetiantiany.cn/gtlsrgdabi.html

[R52] 统计行数
来源：http://hz.jianghu66.top/gtjjebxfrn.html

wc -l a.txt
来源：http://hz.tianlin.xyz/gtbyyzpgxp.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtguiaucdg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtkdvkqtry.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtgwmuyinl.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtoccaezcz.html

[R55] 压缩与解压
来源：http://hz.cucudq.cn/gtgfigwduf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtpzylrdsg.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtokchnkpr.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtcnllujky.html

[R57] 远程执行命令
来源：http://hz.xinyue.icu/gtwkczywoh.html

ssh user@host 'uptime'
来源：http://hz.yj20258.top/gtktajolsz.html

[R58] 下载文件
来源：http://hz.316326.xyz/gtjatgzznm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.haohaochexian.top/gtydtdrumo.html

[R59] 发 POST JSON
来源：http://hz.cheryme.top/gtqhqxpnny.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yvedp.cn/gtjxqvosfe.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtyselwfup.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtqufcuqib.html

[R61] 磁盘占用
来源：http://hz.jyoumei.cn/gtirhjokyx.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gtpnzwlhjs.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtqjuuhccw.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtawmtkogf.html

[R63] 内存与进程
来源：http://hz.jqgufenzy.top/gtzqfzuivt.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtjptcnvuq.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtacrcmjqr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtaadlcwoa.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtmxbmrnrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtjavntnmb.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gtdymiclhd.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtrojxprel.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtiqcevcpr.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtynbbiqmc.html

[R68] 计算文件校验值
来源：http://hz.yj20258888.top/gtefzuatfc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtlwbahgtv.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtfmgkifzc.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtjwpayncr.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtfqytdtgh.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtzvvjtlrr.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtivoazfqy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pengpengdd.cyou/gtvnqlxvaj.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtyaodnhdf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtcusshiym.html

[R73] 分割大日志
来源：http://hz.yueranfly.top/gtcizlqfkt.html


<!-- 参考信息 -->