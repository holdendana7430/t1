代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.chenzaomai.com/gtpaeggeqm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.haohaochexian.top/gtyeroqmlf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shuidangran.top/gtfyhyzfqy.html

[Q15] 查询全部
来源：http://hz.yangfankeji.com/gtnkmrtbwf.html

SELECT * FROM users;
来源：http://hz.pengpengdd.cyou/gtiibgdcig.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtvjmdogvl.html

SELECT id, name FROM users;
来源：http://hz.ehwqpu.com/gtqnvbgkto.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtehdoomwy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.birdmap.top/gtrqbtituo.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtybflxspz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtkgwmjuhi.html

[Q19] 范围查询
来源：http://hz.ybcxt.top/gtwvqhekum.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gtgkbobzkv.html

[Q20] IN 列表
来源：http://hz.iojbl.cn/gtypggnstf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hnxiangtu.top/gtbjzmcbxx.html

[Q21] 空值判断
来源：http://hz.pengpengdd.cyou/gtlvvetvom.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.kuanghao11.cn/gtealikbou.html

[Q22] 排序
来源：http://hz.jinghuilouyu.cn/gtjtkygtdh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtguqrthie.html

[Q23] 分页
来源：http://hz.yuanzhike.top/gttyxpvanx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sufxvd.cn/gtniafmqjm.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtuhasajvd.html

SELECT DISTINCT city FROM users;
来源：http://hz.sufxvd.cn/gtvjqmlznk.html

[Q25] 只取前 N 条
来源：http://hz.cheryme.top/gtvrjrugfp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gtbkxymnxk.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gtwetnsdis.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuetiantiany.cn/gtcbwddupc.html

[Q27] 条件计数
来源：http://hz.cashguo.top/gtembmaakt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtutmiriul.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtjkwhjobb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtgvxnrjne.html

[Q29] 最大最小值
来源：http://hz.zhengqikj.top/gtdacwcrqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cqqwz.cn/gthhlynkqz.html

[Q30] 分组统计
来源：http://hz.sweek.top/gtrkwbpjvn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtzglplsbj.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangtech.top/gtsexzbbfz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.bjfxy.top/gtdcoqkpju.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtbwxtywrw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtkswonype.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtypwbkbph.html

[Q33] 多列分组
来源：http://hz.chenlongwang.top/gtnvjctnuo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtynfvrncc.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtqogafitf.html

SELECT * FROM (
来源：http://hz.ivvv.top/gteoxkzbfo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pengpengdd.cyou/gtsfbrlery.html

) t WHERE rn = 1;
来源：http://hz.jinqigfzy.top/gtdurbazfw.html

[Q35] 内连接
来源：http://hz.jiagoushi.top/gtziarjcpr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtpcvnzlhg.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtjllcjtxx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtxkhdnpoy.html

[Q37] 右连接
来源：http://hz.guannengcc.top/gtvvrbbluv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtdthngohv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pycfn.com/gtabmbxvoc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtxerlicxb.html

[Q39] 自连接（查上下级）
来源：http://hz.iojbl.cn/gtebbnnpuw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ppjwa.cn/gtvovavsbw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtmgybctzw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtomfemkny.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhijiandao.cn/gtyecwlozg.html

[Q41] 多表连接
来源：http://hz.andypj.xyz/gtkymkvaem.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dashuyun.cn/gtoucosunq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtkjdqvpge.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhijiandao.cn/gtrmwsdqio.html

[Q42] 连接条件附加过滤
来源：http://hz.haohaochexian.top/gtefmlhddz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtdjnzimmo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aibaodan.cn/gtaxrctzwg.html

[Q43] 标量子查询
来源：http://hz.xylfe.cn/gtpkcweska.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sxryk.cn/gtljsnouad.html

[Q44] IN 子查询
来源：http://hz.fengsongda.top/gtqyoeldgr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtizghpgvt.html

[Q45] EXISTS 判断存在
来源：http://hz.gaohongyu789.top/gtalxzvynp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtxbqnxqha.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtnrwrzorv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtgshhwppn.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gthradzuoj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dashuyun.cn/gtaxuqjtgt.html

[Q48] CTE 公用表表达式
来源：http://hz.jiagoushi.top/gtfacjrfjq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gttsjocgqw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtewufspci.html

[Q49] 更新单行
来源：http://hz.yj20258.top/gtgohhuafz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtackoakuy.html

[Q50] 批量更新
来源：http://hz.yonumen.top/gtggtnjxsq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gzhubu.top/gtleafvupp.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtldolylkt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuanzx.com/gtwygsxkss.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gtzjyvanrf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shuidangran.top/gtbmskpojt.html

[Q53] 按条件删除
来源：http://hz.hywenlv.cn/gtuulqcwak.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtpncipqtc.html

[Q54] 清空表
来源：http://hz.ywan-chungtsiang.top/gtgbeoowho.html

TRUNCATE TABLE logs;
来源：http://hz.xylfe.cn/gteegesarv.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtaoitwgmw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtntstcfzc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gtccryapxh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtsmoatrmh.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtskekvzox.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtoparaqzd.html

[Q58] 累计求和
来源：http://hz.tianlin.xyz/gtfgikdckp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.9152youxi.cn/gtihjyukmd.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gttudxgxdb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xinyue.icu/gtcvoubena.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnxiangtu.top/gthsmrsrvs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.mhx1999.top/gtdhvmovgi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtwnghpzdg.html

[Q61] 移动平均
来源：http://hz.jianghu66.top/gtzhpztikz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtngohscgi.html

[Q62] 分组占比
来源：http://hz.ybcxt.top/gtrqkqcuka.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtmxwimgaf.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gthmhjtdrw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gtcnfwmjhp.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gtrtdsdidx.html

COMMIT;
来源：http://hz.zhongyouzk.top/gteevirgre.html

[Q65] 回滚事务
来源：http://hz.tanke756.top/gtjnqvhcza.html

ROLLBACK;
来源：http://hz.xuetiantiany.cn/gttbkidmyt.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtizerercs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangkeji.top/gtuoqydrjn.html

[Q67] 设置隔离级别
来源：http://hz.shuidangran.top/gtxddocxwu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtlgwewxet.html

[Q68] 保存点
来源：http://hz.smart0.xyz/gttifydmak.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtcpikskho.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtburypsez.html

[Q69] 查看执行计划
来源：http://hz.jinghuilouyu.cn/gtmimojesh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtffbcjswj.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gtkjztwedt.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtsaqgzouj.html

[Q71] 查看建表语句
来源：http://hz.xziqi.cn/gtiasznnrv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtxifyajzg.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtwapgagzn.html

SHOW INDEX FROM users;
来源：http://hz.sysykeji.top/gtdfcutmqk.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangtech.top/gtvewwzkvz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtfcijaoud.html

[Q74] 强制使用索引
来源：http://hz.yj20258.top/gtyccbabgp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinyuanbaomall.cn/gtseeusazh.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtqlqasvqq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangtech.top/gtqvbgisrx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtqqysbpva.html

[Q76] 按天统计
来源：http://hz.zdqjudy.top/gtcnksiqvm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hammf.cn/gtdolvkftm.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gtcatdjaws.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gaohongyu789.top/gtxgrvsape.html

[Q78] 当前时间
来源：http://hz.hongshengwenyu.top/gtyzbrmoil.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hammf.cn/gtjjfpyffh.html

[Q79] 字符串拼接
来源：http://hz.redwolf501.top/gtoshgxgud.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtqshtkztg.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtaicqwnvb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pycfn.com/gtrbcahbfu.html

[Q81] 字符串替换
来源：http://hz.zdqjudy.top/gtithrkzay.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gtgsgxitce.html

[Q82] 字符长度与字节长度
来源：http://hz.9152youxi.cn/gtxfaikmme.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gaohongyu789.top/gtcgcahwyz.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtpbdbfkim.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tian-w.cn/gtuwewzpnn.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtlfqvdegh.html

SELECT TRIM(name) FROM users;
来源：http://hz.sysykeji.top/gtvmfclgga.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gtuojmypqe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtzaguwlxm.html

[Q86] 读取 JSON 字段
来源：http://hz.redwolf501.top/gtdneaiyng.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtqwsxdrms.html

[Q87] JSON 字段做条件
来源：http://hz.dianchejie.cn/gtfverpqcc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtrclmhena.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtyjzosejd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ybcxt.top/gtvmffnggu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigfzy.top/gtvjoowukf.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtjbfylnfh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.mhx1999.top/gtlnfzufxg.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtvevzgmqx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtvwujctpg.html

================================================================================
来源：http://hz.tianlin.xyz/gtbcplqmry.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gtreqfztuk.html

================================================================================
来源：http://hz.aibaodan.cn/gtukfgsbpk.html

[R01] shebang 与严格模式
来源：http://hz.daxiang520.top/gtmfebfhut.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtclinymjq.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gtrckveibp.html

[R02] 变量赋值与使用
来源：http://hz.wangshuangyany.cn/gtuqodspnv.html

name="Tom"; echo "$name"
来源：http://hz.xziqi.cn/gtemnlzgit.html

[R03] 只读变量
来源：http://hz.jinqigufen.top/gtmikzlixv.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtsqcylyxw.html

[R04] 位置参数
来源：http://hz.yongpay.top/gtugyncwdl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gaohongyu789.top/gtlgdxunhm.html

[R05] 参数默认值
来源：http://hz.dianchejie.cn/gtvottrzhc.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtmypwhcvo.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtmsavtjle.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtjajxdgpd.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gtqqxvwufj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yueranfly.top/gtvsgyobfw.html

[R08] 数值比较
来源：http://hz.nanxinkj.top/gtgotvwwxt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtcunlzzwo.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtcniudpze.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hammf.cn/gtlvbllrtw.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtdntfzghs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtturmodvy.html

[R11] case 多分支
来源：http://hz.shanyushiyangkeji.top/gtfkkdytjs.html

case "$1" in
来源：http://hz.haohaochexian.top/gtykrpduil.html

start) echo "启动" ;;
来源：http://hz.chenzaomai.com/gtzmnctkoc.html

stop)  echo "停止" ;;
来源：http://hz.gogol.net.cn/gtbvhmfmqh.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gtlikbragd.html

esac
来源：http://hz.jinqigfzy.top/gtnbrihgzg.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gttycyhxtc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtynsdvlqn.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtwayqelbk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtbthsqrta.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gthoofukqz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gtxjybwmwn.html

[R15] while 逐行读文件
来源：http://hz.chenjidiqi.icu/gtsbsxfkeq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.svipenyu.cn/gtnafhwszr.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gttdhcroaw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guowangkeji.top/gtchxaqejp.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtqiqzflnb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gtvxyyvwds.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtbgddnzit.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtjkfjicgi.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtxsvvvbbb.html

echo "${#arr[@]}"
来源：http://hz.shuidangran.top/gtpgnlozdq.html

[R20] 关联数组（字典）
来源：http://hz.shangyingyoupin.top/gtahzmcnvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gtwyioidoz.html

[R21] 字符串长度
来源：http://hz.yonumen.top/gttemdvmvo.html

echo "${#s}"
来源：http://hz.xuanzx.com/gtksrczfmq.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtzbcyjzve.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtkmauitaq.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gtsgfunpzm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuanzhike.top/gtezmkppse.html

[R24] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtcbecmudw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ehwqpu.com/gtxsazbofa.html

[R25] 去后缀 / 去前缀
来源：http://hz.kuanghao11.cn/gtunknkbtf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtrdovidip.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtwknntpjs.html

now=$(date +%F); echo "$now"
来源：http://hz.yonumen.top/gtehvcbgwc.html

[R27] 算术展开
来源：http://hz.yueranfly.top/gtrirgglsl.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtnkuehxru.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtkxzlqpyz.html

echo "scale=2; 10/3" | bc
来源：http://hz.xziqi.cn/gtsepduxwu.html

[R29] 定义函数
来源：http://hz.tanke756.top/gttostiilt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangkeji.top/gtsewmujru.html

[R30] 函数返回状态码
来源：http://hz.yuanzhike.top/gtgsxugxxz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtzxlqmwnc.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtvwalcxoh.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtekaijawt.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtdqcodnnp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuanzhike.top/gtaxiedqww.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gtawxbfqcq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtkujtvaci.html

[R34] 退出时清理
来源：http://hz.chenlongwang.top/gtuxqozwpi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtfzozrbvp.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtxnpceupi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtuplrdvph.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gteqzicjsn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtsutvxjsc.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gtamjccvhd.html

files=$(ls -1)
来源：http://hz.sweek.top/gttregipxr.html

[R38] 管道串联
来源：http://hz.vqdsnc.cn/gtatqtwdnt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtjupvvcng.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtcghujgdc.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtnzvsfaxg.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtqjfubcyn.html

echo "log" >> out.log
来源：http://hz.guannengcc.top/gtdglblite.html

[R41] 丢弃输出
来源：http://hz.shuidangran.top/gtdkaefinl.html

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtyxiyqipk.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gtwmjpdydj.html

wc -l < a.txt
来源：http://hz.vqdsnc.cn/gtiqgcdmkn.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtksgduber.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtxjfqxoro.html

[R44] 按修改时间查找
来源：http://hz.daria6918.cn/gtokkcjbgu.html

find . -mtime -7 -type f
来源：http://hz.yj202588.top/gtnvhibsmj.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtgflvhlmc.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtnqdkxjxh.html

[R46] 递归替换文件内容
来源：http://hz.kuanghao11.cn/gtriiiopfu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gtybdmbnag.html

[R47] sed 单行替换
来源：http://hz.redwolf501.top/gtgkkzfzja.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.9152youxi.cn/gthwfdnkjb.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtxceewcee.html

awk '{print $1, $3}' a.txt
来源：http://hz.ppjwa.cn/gtwksatyns.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtomnijrts.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtvghqmnzj.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtnvhicmhp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daxiang520.top/gtovkrfgii.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gtswxjjqfo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtnhcwylmn.html

[R52] 统计行数
来源：http://hz.zycfv.cn/gtgrltwtis.html

wc -l a.txt
来源：http://hz.meibo888.top/gtpbktxeta.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtjiokyqgi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guowangkeji.top/gteajqhacr.html

[R54] 比较两个文件
来源：http://hz.birdmap.top/gtyixipyzm.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtrkxldvfo.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtjjffwdno.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jyoumei.cn/gtassgwalf.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtiiinnity.html

scp file user@host:/path/
来源：http://hz.jinyuanbaomall.cn/gtqecyfpis.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtokrmkooi.html

ssh user@host 'uptime'
来源：http://hz.jiagoushi.top/gtzgtxftkp.html

[R58] 下载文件
来源：http://hz.yuanzhike.top/gtstyppyis.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydjk.org.cn/gtbvhlsdqf.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtfqeiryhn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtdjyoywoo.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtarhbjrjn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gteiuydxne.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gttxkuuftn.html

df -h;  du -sh *
来源：http://hz.pengpengdd.cyou/gtsjfvkvgb.html

[R62] 找最占空间的文件
来源：http://hz.c1oappe.top/gtlusqdhet.html

du -ah . | sort -rh | head -10
来源：http://hz.meibo888.top/gttcamlgvh.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gtsebfwhjc.html


<!-- 参考信息 -->