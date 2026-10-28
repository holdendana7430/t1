代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.haohaochexian.top/gttydiyjlf.html

[Q20] IN 列表
来源：http://hz.cdnleiting.top/gtwvbcbxnu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pycfn.com/gtffoauygm.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtskhmeuej.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ywan-chungtsiang.top/gtcqlfbuqu.html

[Q22] 排序
来源：http://hz.shuidangran.top/gtnndiavdq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.daxiang520.top/gtmfpxienr.html

[Q23] 分页
来源：http://hz.zhijiandao.cn/gtqpyythur.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nwbrower.top/gtcajlagyd.html

[Q24] 去重
来源：http://hz.zhiwuduotai.top/gthbelwkhr.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtrcujwqdb.html

[Q25] 只取前 N 条
来源：http://hz.wangdashe.top/gtvsharkeo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtxywzcwpv.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtomgxxxme.html

SELECT COUNT(*) FROM users;
来源：http://hz.tanke756.top/gtzshteguq.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtzcwzudwd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtokracirv.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtrqfhqeib.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtpslmodrf.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtkitmqrmh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtywhatnng.html

[Q30] 分组统计
来源：http://hz.chenzaomai.com/gtghwdepxc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtomilnxzd.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtahzdnsck.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shzxlz.cn/gttghqkpps.html

[Q32] 分组拼接字符串
来源：http://hz.ivvv.top/gtcyjyvgqh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtpudrqqme.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gogol.net.cn/gtabfwqaoo.html

[Q33] 多列分组
来源：http://hz.yanxiufei.cn/gtuehhtnwv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuxming.cn/gtdtluwuqj.html

[Q34] 每组取第一条
来源：http://hz.cheryme.top/gtjtblywnk.html

SELECT * FROM (
来源：http://hz.feifeiyinyue.top/gtapgflvwi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hywenlv.cn/gtlwsmvibq.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gtmohmhhhy.html

[Q35] 内连接
来源：http://hz.xuanzx.com/gtbpzfnzdo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtuiixohnj.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtjjtlvuan.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gtqognmahq.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtvfwgorqj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jlsjyb.cn/gtgdxojwfk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinqigufen.top/gtthtroawy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tianlin.xyz/gtkzwzwudt.html

[Q39] 自连接（查上下级）
来源：http://hz.shuidangran.top/gtmdsipntm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.vqdsnc.cn/gtdhjwektu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.meibo888.top/gtvbvzenlv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gtclkhrlgc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtltuvnmux.html

[Q41] 多表连接
来源：http://hz.jyoumei.cn/gtgntsoxsv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xingfuxueyuan.xyz/gtyekctpdn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtcdczemvh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtyvygpxih.html

[Q42] 连接条件附加过滤
来源：http://hz.mhx1999.top/gtktbckhdn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtwpeaicfh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtobustrrb.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gtjjqfcgom.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sweek.top/gtxxcgtsdf.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtmiibavhk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ehwqpu.com/gtjawodxfy.html

[Q45] EXISTS 判断存在
来源：http://hz.hammf.cn/gtjbwmdhyt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtpuyiqwtg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.snrcjt.cn/gthyztlpzs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gttanqvhyu.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtvizekvap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhongyouzk.top/gtbqlogiyt.html

[Q48] CTE 公用表表达式
来源：http://hz.guannengcc.top/gtptjxcusx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gtvjggdjjn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fengsongda.top/gtaxklzmee.html

[Q49] 更新单行
来源：http://hz.xinyue.icu/gtbubaqwnr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cdnleiting.top/gtfujloiue.html

[Q50] 批量更新
来源：http://hz.xuanzx.com/gtcvoenyyq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sxryk.cn/gtnttlmrwc.html

[Q51] 用子查询更新
来源：http://hz.quarkkingdee.top/gtnesjrybn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhoulong.xyz/gtavhyusut.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtwrfqsgqo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtlvxqfbue.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtqkvcrqlk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.haohaochexian.top/gtsscltbkp.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtlmecdjry.html

TRUNCATE TABLE logs;
来源：http://hz.iojbl.cn/gtlpxxhpyb.html

[Q55] 排名（并列占位）
来源：http://hz.gogol.net.cn/gtotoigyxo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gteqlsuwfv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxinkj.top/gtljgsccsd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtekkwmqkc.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtfuinqqeh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtrgfvavcz.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtmwfdnkem.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ehwqpu.com/gtiapvreuo.html

[Q59] 分组内累计
来源：http://hz.cashguo.top/gtezqivizq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gtzsxvgfxv.html

[Q60] 取上一行 / 下一行
来源：http://hz.gogol.net.cn/gtyujqncpj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtbzgmmnac.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.kuanghao11.cn/gtwghkcasy.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtyuenumwf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtfgckttqx.html

[Q62] 分组占比
来源：http://hz.nanxinkj.top/gtkkaatzin.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtqhfhdxbl.html

[Q63] 开启事务
来源：http://hz.zhengqikj.top/gtgcxqglpc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cucudq.cn/gtqtvhyujk.html

[Q64] 提交事务
来源：http://hz.hywenlv.cn/gtxfmuvndp.html

COMMIT;
来源：http://hz.sxryk.cn/gtjejditgi.html

[Q65] 回滚事务
来源：http://hz.9152youxi.cn/gtvuebuqtu.html

ROLLBACK;
来源：http://hz.nanxinkj.top/gtghcopgze.html

[Q66] 行锁查询
来源：http://hz.gzhubu.top/gtlfujmrgh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nwbrower.top/gtichcjfrs.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtvrnmnlwi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtncypmypr.html

[Q68] 保存点
来源：http://hz.zhiwuduotai.top/gtjfagagsf.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtsaynyrpm.html

ROLLBACK TO sp1;
来源：http://hz.zhengqikj.top/gtigvbszde.html

[Q69] 查看执行计划
来源：http://hz.tianlin.xyz/gtfaaoitje.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.havefunace.top/gtjidqbrvp.html

[Q70] 更新统计信息
来源：http://hz.shangyingyoupin.top/gtlwnwddwc.html

ANALYZE TABLE users;
来源：http://hz.aibaodan.cn/gtjtqpidfi.html

[Q71] 查看建表语句
来源：http://hz.jinyuanbaomall.cn/gtfurrjhbw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gtberakuzp.html

[Q72] 查看索引
来源：http://hz.jyoumei.cn/gtihhdgmll.html

SHOW INDEX FROM users;
来源：http://hz.daria6918.cn/gtsqxgowun.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gtkrbbntge.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dianchejie.cn/gtrymoiore.html

[Q74] 强制使用索引
来源：http://hz.fengsongda.top/gtazwnsozs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtxhmeboaw.html

[Q75] 日期格式化
来源：http://hz.chenlongwang.top/gtxohbnzat.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangshuangyany.cn/gtytjomvyj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinqigfzy.top/gtexxrstab.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtmsvpntcp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.316326.xyz/gtaelrkacx.html

[Q77] 时间加减
来源：http://hz.cheryme.top/gtuwpfttun.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gteupgjnbm.html

[Q78] 当前时间
来源：http://hz.jinghuilouyu.cn/gtmrkmonvz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yonumen.top/gtfqpydqcd.html

[Q79] 字符串拼接
来源：http://hz.yonumen.top/gtxczvrurk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aibaodan.cn/gttciwgtbs.html

[Q80] 字符串截取
来源：http://hz.cqqwz.cn/gthhadioxo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxuanxn.top/gtqkuzfkxe.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtqiyaaboq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtabztgewh.html

[Q82] 字符长度与字节长度
来源：http://hz.ydzc1.top/gtsfklqyyw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnxiangtu.top/gtxqykuomr.html

[Q83] 大小写转换
来源：http://hz.gaohongyu789.top/gtcueqdmue.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtgtoqjypr.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtaitknoet.html

SELECT TRIM(name) FROM users;
来源：http://hz.aibaodan.cn/gtmobsskvr.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtajxxvfin.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtaqesztjd.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtgcovcvcp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ywan-chungtsiang.top/gtqldbpiox.html

[Q87] JSON 字段做条件
来源：http://hz.wangshuangyany.cn/gthpbackal.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtkugogzpf.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gtmsgzspld.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtuvsqcrpp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhiwuduotai.top/gtyapvvkox.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gtuzjjabwg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtakxfrzie.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtlpgtixqw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtdbrneumg.html

================================================================================
来源：http://hz.jqgfzy.top/gtdbnzyenl.html

R. Bash 专题
来源：http://hz.yuxming.cn/gtcihkakyq.html

================================================================================
来源：http://hz.dashuyun.cn/gtwopatjip.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtrtejjutc.html

#!/usr/bin/env bash
来源：http://hz.ybcxt.top/gtwyzgdbzt.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gtqvxhgzfp.html

[R02] 变量赋值与使用
来源：http://hz.xziqi.cn/gtmbxnitug.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtetwigtya.html

[R03] 只读变量
来源：http://hz.0kj1m.cn/gtpetsezev.html

readonly PI=3.14
来源：http://hz.cdnleiting.top/gthcixfvds.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gtcggmnook.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gtwjglstrn.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtjecwgtya.html

name="${1:-default}"
来源：http://hz.zycfv.cn/gtoqyzemgb.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtodblqjig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtwohaotml.html

[R07] if 判断文件
来源：http://hz.chenlongwang.top/gtxieiouyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtunnttbct.html

[R08] 数值比较
来源：http://hz.daxiang520.top/gteoxhzvmi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtflksrrnq.html

[R09] 字符串比较
来源：http://hz.yvedp.cn/gtxyxmqrtc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtwwrcaevr.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtwcsognrm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtuueddovi.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtjyilfjxz.html

case "$1" in
来源：http://hz.cqqwz.cn/gtxqluubcx.html

start) echo "启动" ;;
来源：http://hz.zhixingplan.top/gtoyxuxhbp.html

stop)  echo "停止" ;;
来源：http://hz.chenjidiqi.icu/gtwrsthwyh.html

*)     echo "未知命令" ;;
来源：http://hz.guowangkeji.top/gtzntxfsic.html

esac
来源：http://hz.ydzc1.top/gtzutikndp.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtrllkqllx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gtglwkfbkv.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtpieggjpp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gttzazqknh.html

[R14] C 风格 for
来源：http://hz.smart0.xyz/gtnaolsscj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtqnulwxdq.html

[R15] while 逐行读文件
来源：http://hz.guowangkeji.top/gtjxjrwpjc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangshuangyany.cn/gtiqvganes.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtseujviip.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gttazdzpaa.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtscckotnr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cheryme.top/gtoanpyjnk.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtglgksime.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtwxtvdcuo.html

[R19] 数组长度
来源：http://hz.tianlin.xyz/gtcffkzdlv.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gteaxhqpmu.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gthoaifzob.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtybxonfvj.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gtbodvwkos.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtmnuwsenk.html

[R22] 截取子串
来源：http://hz.jinqigufen.top/gtfujntfso.html

echo "${s:0:5}"
来源：http://hz.guowangkeji.top/gtidgpelzr.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtukcyhgtw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gthynnoxwn.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtpanltgae.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinyuanbaomall.cn/gtvfqpbvpb.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj202588.top/gticcnssxt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yongpay.top/gtrcgirjqz.html

[R26] 命令替换
来源：http://hz.tanke756.top/gtgvovnxha.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtdybxmqeq.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtqphrygbu.html

echo $((1 + 2 * 3))
来源：http://hz.cashguo.top/gtlwuzrzsg.html

[R28] 浮点运算
来源：http://hz.chenjidiqi.icu/gtyeqduzjs.html

echo "scale=2; 10/3" | bc
来源：http://hz.hongshengwenyu.top/gtcdlezgpd.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtubhobsnx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.mhx1999.top/gtwkpaekrz.html

[R30] 函数返回状态码
来源：http://hz.jinghuilouyu.cn/gtrihcsmpo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtaosjvybg.html

[R31] 局部变量
来源：http://hz.haohaochexian.top/gtkcbiwlhx.html

f() { local x=1; echo "$x"; }
来源：http://hz.svipenyu.cn/gtyheekupy.html

[R32] 参数个数校验
来源：http://hz.wangshuangyany.cn/gtdqihkszj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.birdmap.top/gttacrulpk.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxinkj.top/gtgrcvvxxu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtcbkspswo.html

[R34] 退出时清理
来源：http://hz.zhoulong.xyz/gtmoauvyoe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtxowzhnms.html

[R35] 后台执行并等待
来源：http://hz.iojbl.cn/gtryjystur.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtdryjqgfy.html

[R36] 并发执行多个任务
来源：http://hz.fengsongda.top/gtanxhrhwi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenzaomai.com/gteovokagw.html

[R37] 把输出赋给变量
来源：http://hz.havefunace.top/gtkmsxplen.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtfqikjwtv.html

[R38] 管道串联
来源：http://hz.yj20258.top/gtycvoansn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hfpthk.cn/gtjkaadssg.html

[R39] 重定向标准输出与错误
来源：http://hz.zhaomingkeji.xyz/gtwsopvpfp.html

cmd > out.log 2>&1
来源：http://hz.hnqzz.top/gtfnjhzxlb.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtdqrleetl.html

echo "log" >> out.log
来源：http://hz.cqqwz.cn/gtnpyhubfv.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gtohpnuvmt.html

cmd >/dev/null 2>&1
来源：http://hz.jlsjyb.cn/gtedvuzvvq.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gtcpywdzcr.html

wc -l < a.txt
来源：http://hz.yj20258.top/gtsswiqzde.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtfpbunhml.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtccirwsjb.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtredwpwnf.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtxfancpnn.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtkipqpvdy.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtxdycefde.html

[R46] 递归替换文件内容
来源：http://hz.chenzaomai.com/gtkaogyzdx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gtmterbueb.html

[R47] sed 单行替换
来源：http://hz.c1oappe.top/gtrsasgqgi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtvsdlpqpv.html

[R48] awk 取指定列
来源：http://hz.tanke756.top/gtewhpnfdb.html

awk '{print $1, $3}' a.txt
来源：http://hz.guowangkeji.top/gteyutgqml.html

[R49] awk 带条件
来源：http://hz.bjfxy.top/gtyuvrepvs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtmadxumgb.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtgbvkhcuy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtjzzxujjs.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtcwnnoiuj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.haohaochexian.top/gtnsagytpw.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gtjgxwgcgf.html

wc -l a.txt
来源：http://hz.xuanzx.com/gtkgpavrue.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtobavenjt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtmmqdcumu.html

[R54] 比较两个文件
来源：http://hz.pengpengdd.cyou/gtisvgzmvj.html

diff a.txt b.txt
来源：http://hz.dianchejie.cn/gthulelskw.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtzglvinqk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtilflcxsi.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gthxxhkajp.html

scp file user@host:/path/
来源：http://hz.zhixingplan.top/gtruxsvgzf.html

[R57] 远程执行命令
来源：http://hz.cashguo.top/gtimuxxwlg.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtktizaqsk.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtlhypakol.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zdqjudy.top/gtewsweccw.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtubhxhpdv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ywan-chungtsiang.top/gtwwgnramq.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtezumdzcp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtacxqhaoj.html

[R61] 磁盘占用
来源：http://hz.xinyue.icu/gtnwpjigou.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtkyquicvb.html

[R62] 找最占空间的文件
来源：http://hz.gzhubu.top/gtgoviigot.html

du -ah . | sort -rh | head -10
来源：http://hz.kuanghao11.cn/gtnhggmeab.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtcxyjjlxc.html

free -h;  ps aux | grep nginx
来源：http://hz.bjfxy.top/gtoqxihrkh.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gttittpavo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sysykeji.top/gtadhnhbym.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtzqpqvxwy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnqzz.top/gtkjuelvfm.html

[R66] 定时任务
来源：http://hz.shanyushiyangkeji.top/gtywjeridf.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtykgtkxzf.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtcnpdqdph.html

openssl rand -hex 16
来源：http://hz.xingfuxueyuan.xyz/gtinlrontk.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtxreitfgf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xinyue.icu/gttrclkzna.html

[R69] 生成随机密码
来源：http://hz.hnqzz.top/gtgbierqos.html


<!-- 参考信息 -->