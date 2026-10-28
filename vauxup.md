代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shanyushiyangtech.top/gtutxqkdzg.html

[Q18] 模糊匹配
来源：http://hz.yj202588.top/gtlegodajm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.iojbl.cn/gtyakylzer.html

[Q19] 范围查询
来源：http://hz.redwolf501.top/gtzkrwnrcy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenjidiqi.icu/gtfljvuurn.html

[Q20] IN 列表
来源：http://hz.feifeiyinyue.top/gtkvkbnvfw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinyuanbaomall.cn/gtofnhildd.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gtdmkqvevq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gttnggpsal.html

[Q22] 排序
来源：http://hz.kuanghao11.cn/gtaxsmmenw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.c1oappe.top/gtnysvfthg.html

[Q23] 分页
来源：http://hz.tianlin.xyz/gtozszkrbp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cucudq.cn/gtvguhnxhi.html

[Q24] 去重
来源：http://hz.wangshuangyany.cn/gtkrtfsaqr.html

SELECT DISTINCT city FROM users;
来源：http://hz.guowangkeji.top/gtyierqfti.html

[Q25] 只取前 N 条
来源：http://hz.daxiang520.top/gtoqsttvtp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtdswnfegh.html

[Q26] 计数
来源：http://hz.sufxvd.cn/gtlfrqatns.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtigmfdcpf.html

[Q27] 条件计数
来源：http://hz.ydjk.org.cn/gtvoxlzkqx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhongyouzk.top/gtqosvuqmu.html

[Q28] 求和与平均
来源：http://hz.snrcjt.cn/gthkdsrlue.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtsgylwqby.html

[Q29] 最大最小值
来源：http://hz.pycfn.com/gtltvmdgnx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinghuilouyu.cn/gtslajnomr.html

[Q30] 分组统计
来源：http://hz.ppjwa.cn/gtaypzkwur.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtobkwhslb.html

[Q31] 分组后过滤
来源：http://hz.sxryk.cn/gtyqliyrmf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sweek.top/gtbbdiabxd.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gthxkdrlua.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gttaiiidbx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhongyouzk.top/gtmybgajtw.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtomvrguke.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangtech.top/gturovgubi.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtsqjtfbjz.html

SELECT * FROM (
来源：http://hz.zycfv.cn/gtbietdzqb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aibaodan.cn/gthcbgzdoc.html

) t WHERE rn = 1;
来源：http://hz.jinqigufen.top/gtuldunahk.html

[Q35] 内连接
来源：http://hz.jqgfzy.top/gtrdyjzpmb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtiyvdwzkc.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gtiwitmdyp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shzxlz.cn/gtyxdsolkk.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtnaxxpzki.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuetiantiany.cn/gthseihrfu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtbtlxevng.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhiwuduotai.top/gtooftumwi.html

[Q39] 自连接（查上下级）
来源：http://hz.dianchejie.cn/gtyjwqbygh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cucudq.cn/gtlmzzyvsw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hongshengwenyu.top/gtadaqdurf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangtech.top/gtfjpnybak.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.kuanghao11.cn/gthtttbgad.html

[Q41] 多表连接
来源：http://hz.quarkkingdee.top/gtfkuureda.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.quarkkingdee.top/gtxxhspppo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daria6918.cn/gtkcbgammr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gtzdawhqls.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtzuivgkki.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtapghncjq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xylfe.cn/gtdricalxk.html

[Q43] 标量子查询
来源：http://hz.zhengqikj.top/gtpqfjsmah.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cucudq.cn/gtyftrshcp.html

[Q44] IN 子查询
来源：http://hz.redwolf501.top/gtlrldgckt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtnfdtqwfx.html

[Q45] EXISTS 判断存在
来源：http://hz.tian-w.cn/gtzbjzfymh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtetqoizoz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gtseernfyd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtdrttysth.html

[Q47] 与平均值比较
来源：http://hz.xuanzx.com/gtpekfuoss.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangdashe.top/gtxzivdjso.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gtrjywuqnb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xinyue.icu/gtvjzjqxsg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hywenlv.cn/gtgydhmkyx.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtfrxjqlte.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtdnomvjca.html

[Q50] 批量更新
来源：http://hz.ivvv.top/gtzplbvxqf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aizwys.cn/gtcaqabjix.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtxqvfneqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtbtiwyxxz.html

[Q52] 删除指定行
来源：http://hz.ydjk.org.cn/gtctfiytkf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtrewsdudr.html

[Q53] 按条件删除
来源：http://hz.fzhhl.top/gtjgiqgwyu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xziqi.cn/gtwyaxaqwa.html

[Q54] 清空表
来源：http://hz.svipenyu.cn/gtycwnylwu.html

TRUNCATE TABLE logs;
来源：http://hz.bjfxy.top/gttvypqkup.html

[Q55] 排名（并列占位）
来源：http://hz.ydjk.org.cn/gtwhmtjsit.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtvstyzyce.html

[Q56] 密集排名（并列不占位）
来源：http://hz.iojbl.cn/gtnfsbance.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.iojbl.cn/gtdomnndeb.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtcacljszp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gtclnhdxkh.html

[Q58] 累计求和
来源：http://hz.hfpthk.cn/gtfukjgtqi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.haohaochexian.top/gtcmbneznc.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtvttudlrd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtryewcqlu.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gtcfayagqk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtyfehdrbj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.mhx1999.top/gtpmlxvaay.html

[Q61] 移动平均
来源：http://hz.cqqwz.cn/gtwhrnjehc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtypbijoba.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtdievzpxo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtvrvndqyo.html

[Q63] 开启事务
来源：http://hz.zhengqikj.top/gtxhrpjzdg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yongpay.top/gtlajlllqg.html

[Q64] 提交事务
来源：http://hz.fengsongda.top/gtlondxfex.html

COMMIT;
来源：http://hz.redwolf501.top/gtyfeadwpq.html

[Q65] 回滚事务
来源：http://hz.gogol.net.cn/gtkymctken.html

ROLLBACK;
来源：http://hz.jinghuilouyu.cn/gtithqcoln.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtlviojuep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yanxiufei.cn/gtgzrvlhgx.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtpdttnfpa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gtvxjfocqb.html

[Q68] 保存点
来源：http://hz.gogol.net.cn/gtjagywfxu.html

SAVEPOINT sp1;
来源：http://hz.vqdsnc.cn/gttntdpirm.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtguuotkdq.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtllndzwup.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yvedp.cn/gtypyvghmo.html

[Q70] 更新统计信息
来源：http://hz.feifeiyinyue.top/gtfglkntvz.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtvqwypvmo.html

[Q71] 查看建表语句
来源：http://hz.yj20258.top/gtecxmwybm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtjakoeiwv.html

[Q72] 查看索引
来源：http://hz.zhongyouzk.top/gtuanbesya.html

SHOW INDEX FROM users;
来源：http://hz.hywenlv.cn/gthbmbglik.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangkeji.top/gtdopdjple.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gthpurmovx.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gthtzkvmnq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xingfuxueyuan.xyz/gtptvhgvce.html

[Q75] 日期格式化
来源：http://hz.shangyingyoupin.top/gtmugorlmy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.birdmap.top/gtliidudhp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtzkwnlhra.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtlwhajjnh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xylfe.cn/gtcalieblk.html

[Q77] 时间加减
来源：http://hz.birdmap.top/gthfdhbovf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtgiaewgtc.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtrnstdtya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.vqdsnc.cn/gtehkspclb.html

[Q79] 字符串拼接
来源：http://hz.gogol.net.cn/gtlzhhbqec.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.c1oappe.top/gtodhsvjhi.html

[Q80] 字符串截取
来源：http://hz.zycfv.cn/gtzpgtpdzu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtazfkubhp.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtwzutnhxm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtbtuguolg.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtmhmfkxav.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtupdpakxl.html

[Q83] 大小写转换
来源：http://hz.shzxlz.cn/gtqvlqknyg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenzaomai.com/gttvktsrpo.html

[Q84] 去除首尾空格
来源：http://hz.yuxming.cn/gtkefplohv.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtezllzoow.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtelkvizrt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.bjfxy.top/gtweqenjid.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtihwmkbux.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtplpahxyj.html

[Q87] JSON 字段做条件
来源：http://hz.jqgufenzy.top/gthmxtmkog.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sxryk.cn/gtmrkcmgvi.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnxiangtu.top/gtraxpuyjx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtgjmgsdzv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xinyue.icu/gtjnnuwyho.html

[Q89] 判断表是否存在
来源：http://hz.shzxlz.cn/gttqvgjzdm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gttmtympkm.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtoidoroxa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtpwaowaby.html

================================================================================
来源：http://hz.ydzc1.top/gtgixiovty.html

R. Bash 专题
来源：http://hz.iojbl.cn/gtpcjedpjs.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtolmdkder.html

[R01] shebang 与严格模式
来源：http://hz.zycfv.cn/gtvnhbmchg.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gtwccyjpuj.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtvdskhgnj.html

[R02] 变量赋值与使用
来源：http://hz.yangfankeji.com/gtzyietgbh.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtdbmkplop.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtuwcnrvcy.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtdxiqglxv.html

[R04] 位置参数
来源：http://hz.bjfxy.top/gtjdbehjkz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhijiandao.cn/gtyxbxtktc.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtrmgdywbp.html

name="${1:-default}"
来源：http://hz.xuanzx.com/gtldycurum.html

[R06] 判断命令是否存在
来源：http://hz.cucudq.cn/gtdmchfykw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yongpay.top/gtsodepbic.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtxumxsnvd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuetiantiany.cn/gtwhtagmma.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gtdekfedur.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gthrgzwqyy.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtmmczejbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtpekxbnph.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtjcqajvjm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtyzvvelhr.html

[R11] case 多分支
来源：http://hz.hfpthk.cn/gtcnppyhqe.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtjkkinhjf.html

start) echo "启动" ;;
来源：http://hz.xuanzx.com/gttthqdnbg.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtgpzhzfks.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258888.top/gtcojqqlmd.html

esac
来源：http://hz.wangshuangyany.cn/gtxzspfqqw.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gtyzabbxva.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sysykeji.top/gtxzpchxak.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtahkzqdpj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cashguo.top/gtmxnxdrtr.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtjxitqrma.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtpzgeysvl.html

[R15] while 逐行读文件
来源：http://hz.chenzaomai.com/gtveejizco.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gtcsccpvdh.html

[R16] until 等待条件
来源：http://hz.52xcode.cn/gttdktkuck.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hywenlv.cn/gtuselvbuw.html

[R17] 数组定义与取值
来源：http://hz.zhijiandao.cn/gtedozqebn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jlsjyb.cn/gtjnhavlly.html

[R18] 遍历数组
来源：http://hz.ehwqpu.com/gtkohheqrp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtvopeemwz.html

[R19] 数组长度
来源：http://hz.bjfxy.top/gttlkbkcls.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtqkicrobw.html

[R20] 关联数组（字典）
来源：http://hz.svipenyu.cn/gtxtvqpriv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cdnleiting.top/gtakcclqiq.html

[R21] 字符串长度
来源：http://hz.daxiang520.top/gtnsjdrknw.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtqtbzjynj.html

[R22] 截取子串
来源：http://hz.shuidangran.top/gtiepjtghb.html

echo "${s:0:5}"
来源：http://hz.tianlin.xyz/gtqpkgyugz.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtdcjevhqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtrxzidkzh.html

[R24] 大小写转换
来源：http://hz.jinqigufen.top/gtnscedjgt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtbqhsqrev.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydzc1.top/gtxabuitjn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuanzx.com/gtbvjnjyiy.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtvbhsckpc.html

now=$(date +%F); echo "$now"
来源：http://hz.hnqzz.top/gtxmdbdebr.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtkutrcdnx.html

echo $((1 + 2 * 3))
来源：http://hz.jiagoushi.top/gtgjruqvlo.html

[R28] 浮点运算
来源：http://hz.hnqzz.top/gtyikgipbg.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinqigufen.top/gtwnuwgcqx.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtdjdpsonu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gtuwhvemhp.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtzxhxjhqq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gthvyzzhwg.html

[R31] 局部变量
来源：http://hz.shanyushiyangtech.top/gtkhdqedmp.html

f() { local x=1; echo "$x"; }
来源：http://hz.yongpay.top/gtvvhseucj.html

[R32] 参数个数校验
来源：http://hz.jqgufenzy.top/gtwvtcceka.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgfzy.top/gttsnybkdm.html

[R33] 捕获错误并提示行号
来源：http://hz.zhoulong.xyz/gtkgvlpajo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cheryme.top/gttqozubqf.html

[R34] 退出时清理
来源：http://hz.guowangkeji.top/gtgtruwvuy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtrifcslta.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gtatvulftk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtvjnqjmfo.html

[R36] 并发执行多个任务
来源：http://hz.cheryme.top/gtlqgjeckm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydjk.org.cn/gtomlefjia.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gtfqqwhaow.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtjxqdyonf.html

[R38] 管道串联
来源：http://hz.daria6918.cn/gtncllwefu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gttpgkpltw.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtskdpvwel.html

cmd > out.log 2>&1
来源：http://hz.hammf.cn/gtpdmbpmjn.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtcpzszqpc.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtruugaueq.html

[R41] 丢弃输出
来源：http://hz.zhoulong.xyz/gtfhmnaqhk.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtcfvrcrjp.html

[R42] 输入重定向
来源：http://hz.zhaomingkeji.xyz/gtdhliotfs.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtivoorsjz.html

[R43] 按名字查找文件
来源：http://hz.xylfe.cn/gthdhektuv.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtbzttcxpf.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtavktztgv.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gtlfalnovy.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtoxbrwtpu.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtryidjjkl.html

[R46] 递归替换文件内容
来源：http://hz.52xcode.cn/gthmiklsla.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtvnbtylpq.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gtofzfbnwq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhengqikj.top/gtorndqnxt.html

[R48] awk 取指定列
来源：http://hz.haohaochexian.top/gtmcailuyq.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtmedpcbzz.html

[R49] awk 带条件
来源：http://hz.zhijiandao.cn/gtybcmrqjw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtaudtlocu.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtqenjniil.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtymvyhcom.html

[R51] 排序去重取前几
来源：http://hz.zdqjudy.top/gtbhdqrfvb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhongyouzk.top/gtqhyvwqtc.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtygygklgs.html

wc -l a.txt
来源：http://hz.pengpengdd.cyou/gtdxlfthmn.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtbacqepyw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtxavqrelu.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtxmpuexud.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtqmidpicr.html

[R55] 压缩与解压
来源：http://hz.9152youxi.cn/gtwfnlmoio.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xziqi.cn/gtqfkczgcc.html

[R56] 远程拷贝
来源：http://hz.hywenlv.cn/gtssfrkxvl.html

scp file user@host:/path/
来源：http://hz.yonumen.top/gtkljjggao.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtpqgowcla.html

ssh user@host 'uptime'
来源：http://hz.jinqigufen.top/gtrixthraa.html

[R58] 下载文件
来源：http://hz.jinyuanbaomall.cn/gttqjmugfx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gttqkosmpo.html

[R59] 发 POST JSON
来源：http://hz.0kj1m.cn/gtzrounhgx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.snrcjt.cn/gtlkfsbdnh.html

[R60] 只看 HTTP 状态码
来源：http://hz.ivvv.top/gtkdxcadmr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.meibo888.top/gtibhptepl.html

[R61] 磁盘占用
来源：http://hz.zhaomingkeji.xyz/gtualcjlpg.html

df -h;  du -sh *
来源：http://hz.zhengqikj.top/gtiwcfornr.html

[R62] 找最占空间的文件
来源：http://hz.andypj.xyz/gtvukkypkx.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtwtsldusc.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtkydjdrbv.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtcylojzpo.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtxulbnfei.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydzc1.top/gtxhzoaoux.html

[R65] 查看端口占用
来源：http://hz.jiagoushi.top/gtxzoethji.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnxiangtu.top/gtfcigsypx.html

[R66] 定时任务
来源：http://hz.shzxlz.cn/gtvuagjpfq.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtnovorasr.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtmpnjszod.html


<!-- 参考信息 -->