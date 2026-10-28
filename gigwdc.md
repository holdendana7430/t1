代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtqszxkmwm.html

[Q11] 一次插入多行
来源：http://hz.tianlin.xyz/gtscdcbgid.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangshuangyany.cn/gtfuepluam.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangtech.top/gtgcxznezf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgufenzy.top/gtmmnttnto.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ybcxt.top/gtzokyltjs.html

[Q13] 忽略重复插入
来源：http://hz.zhiwuduotai.top/gtlndhtzot.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gtmktvxqod.html

[Q14] 存在则更新（upsert）
来源：http://hz.shangyingyoupin.top/gtsyhurrax.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jiagoushi.top/gtphhrlktp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgfzy.top/gtemhaxdfl.html

[Q15] 查询全部
来源：http://hz.zhijiandao.cn/gtodqxevzh.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtgcazsthg.html

[Q16] 查询指定列
来源：http://hz.zhongyouzk.top/gtyzmmylzy.html

SELECT id, name FROM users;
来源：http://hz.xziqi.cn/gtqqdujynj.html

[Q17] 条件查询
来源：http://hz.hongshengwenyu.top/gtqknmocye.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenlongwang.top/gtoiidaftt.html

[Q18] 模糊匹配
来源：http://hz.redwolf501.top/gtzamxdutz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gtxhmgnkjg.html

[Q19] 范围查询
来源：http://hz.jqgfzy.top/gtfehuptqe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cashguo.top/gthdfujiwm.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gtceaayxqq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtudzcaxdl.html

[Q21] 空值判断
来源：http://hz.fzhhl.top/gtsuxadvpr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zycfv.cn/gtzyrwgxgk.html

[Q22] 排序
来源：http://hz.yj202588.top/gtcxoxlzsm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.smart0.xyz/gtdsvoyycp.html

[Q23] 分页
来源：http://hz.yj20258.top/gtacssxbzb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sxryk.cn/gteubqlbnp.html

[Q24] 去重
来源：http://hz.pycfn.com/gtakmtkeah.html

SELECT DISTINCT city FROM users;
来源：http://hz.daxiang520.top/gthwdhhhri.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtiadkrmol.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtdsiytqpv.html

[Q26] 计数
来源：http://hz.hywenlv.cn/gtpzkravhj.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtwportmud.html

[Q27] 条件计数
来源：http://hz.chenjidiqi.icu/gtdtiitgdc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yangfankeji.com/gtsjkqxwgw.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtpqmojbkg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gogol.net.cn/gtohcncbca.html

[Q29] 最大最小值
来源：http://hz.ppjwa.cn/gtcxibnqfy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtknitzhmq.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtxjsojqes.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gthyowjafk.html

[Q31] 分组后过滤
来源：http://hz.ybcxt.top/gtmbqdabdj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtzdssotpk.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtffyefbyv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtizwdytyt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cashguo.top/gtfpcrotzu.html

[Q33] 多列分组
来源：http://hz.feifeiyinyue.top/gtzyexalbn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhoulong.xyz/gtbdbskhno.html

[Q34] 每组取第一条
来源：http://hz.yvedp.cn/gtfdlljttf.html

SELECT * FROM (
来源：http://hz.gzhubu.top/gtltzaxbew.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daxiang520.top/gtcbvcteoi.html

) t WHERE rn = 1;
来源：http://hz.jinqigfzy.top/gtbnjytbzj.html

[Q35] 内连接
来源：http://hz.cashguo.top/gtisqxxwwh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtkyiolerz.html

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtkzgllaof.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtlewravfs.html

[Q37] 右连接
来源：http://hz.quarkkingdee.top/gtdfxpqjas.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.iojbl.cn/gtzzxtbnbt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gotoacloud.top/gtfxnenmxk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jqgufenzy.top/gtgyjhnoxx.html

[Q39] 自连接（查上下级）
来源：http://hz.yj202588.top/gtnbgvheii.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.daria6918.cn/gtgnmdkqgo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnxiangtu.top/gturiiihrh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtgayzpsuf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtytytuhga.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtieejzgty.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shangyingyoupin.top/gtlovcgspn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtveprswtu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.guannengcc.top/gtsangnpha.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtidfmzvct.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenlongwang.top/gtrklkmhfv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenzaomai.com/gtxmtuzxup.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtfxehwpnj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gzhubu.top/gtyhikvzef.html

[Q44] IN 子查询
来源：http://hz.wangdashe.top/gtmvhneqmv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.haohaochexian.top/gtyljkjhlf.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtbyctvlrj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gtixfbwkyk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgufenzy.top/gtphwfcurx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtrqewwwrq.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gthhsgxbrm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtizcgzqgk.html

[Q48] CTE 公用表表达式
来源：http://hz.jyoumei.cn/gtjhtbkhwm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gtfuicvtja.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gtmhmpcetb.html

[Q49] 更新单行
来源：http://hz.316326.xyz/gtoivxildf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gtxalxfefe.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtzojaoohx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtpibzunys.html

[Q51] 用子查询更新
来源：http://hz.shanyushiyangtech.top/gtvyedwnkp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtdgxycefz.html

[Q52] 删除指定行
来源：http://hz.9152youxi.cn/gtvfvgvxfj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.quarkkingdee.top/gthyvkjtob.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtviodzyft.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtqnlaznsx.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtlzsbhkqj.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtdyxnssgd.html

[Q55] 排名（并列占位）
来源：http://hz.hammf.cn/gtegyqywcq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gtwesvitch.html

[Q56] 密集排名（并列不占位）
来源：http://hz.snrcjt.cn/gtcxslwhza.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gtftrdvust.html

[Q57] 行号
来源：http://hz.guannengcc.top/gtmopdqatt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gtplwawtfq.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtdgfppnhr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hongshengwenyu.top/gtysqgwekl.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtwrczbscs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yongpay.top/gtljasfnan.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gtvoztoska.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.quarkkingdee.top/gtclnefmst.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtuifbhoiw.html

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtyyspxyfj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhijiandao.cn/gtdgtfousr.html

[Q62] 分组占比
来源：http://hz.sweek.top/gtysbczals.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtckkzmzpe.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gttnbdgrgs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cucudq.cn/gtnumgdjiw.html

[Q64] 提交事务
来源：http://hz.ywan-chungtsiang.top/gtdehaijdj.html

COMMIT;
来源：http://hz.gotoacloud.top/gtgzhougqa.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtkjtejoet.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtzfolzbat.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtrphdcodu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtwzshungs.html

[Q67] 设置隔离级别
来源：http://hz.xinyue.icu/gtjwtfwvya.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtzmpzyqin.html

[Q68] 保存点
来源：http://hz.cheryme.top/gtrjopdnmf.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtdbjtegdc.html

ROLLBACK TO sp1;
来源：http://hz.jinqigufen.top/gtjklhhvrb.html

[Q69] 查看执行计划
来源：http://hz.zhijiandao.cn/gtqrulwimf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuxming.cn/gthgffeksp.html

[Q70] 更新统计信息
来源：http://hz.ywan-chungtsiang.top/gtjwwbkmgk.html

ANALYZE TABLE users;
来源：http://hz.ywan-chungtsiang.top/gtxmkeamar.html

[Q71] 查看建表语句
来源：http://hz.guannengcc.top/gtghbrebmw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hammf.cn/gtnggommbh.html

[Q72] 查看索引
来源：http://hz.shangyingyoupin.top/gttcbjcvvg.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtraarfzls.html

[Q73] 查看表状态
来源：http://hz.cashguo.top/gtonlntztu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gtenzcfnfm.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtxtjedijf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sysykeji.top/gtekogvovq.html

[Q75] 日期格式化
来源：http://hz.cashguo.top/gtzeybdrqr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xylfe.cn/gtdrpfnqhr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.0kj1m.cn/gtpctnrtvq.html

[Q76] 按天统计
来源：http://hz.xylfe.cn/gtqjntzamf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtmgyqtkoc.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtookhyhqo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zdqjudy.top/gtsnhoeuav.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtfjgjfwok.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gtlvewyvni.html

[Q79] 字符串拼接
来源：http://hz.tianlin.xyz/gtixevmfxy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ybcxt.top/gtvanclkez.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtxtxkpkzp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.kuanghao11.cn/gtojovdxfh.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtsfiqmtft.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.fengsongda.top/gtoyjqeadr.html

[Q82] 字符长度与字节长度
来源：http://hz.jyoumei.cn/gtmvwmhznr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.snrcjt.cn/gterysgnof.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtrwhmbfvs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtsueooxux.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtfxbcrgbp.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtxqjiyono.html

[Q85] 数值取整
来源：http://hz.hongshengwenyu.top/gtdwmwtumk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aibaodan.cn/gtvcbvfckf.html

[Q86] 读取 JSON 字段
来源：http://hz.ydzc1.top/gtehbdayic.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuanzx.com/gtjdcmomwx.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtdgnlzmnv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtlpdvaokh.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgufenzy.top/gtmmubdkub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sxryk.cn/gteucesznz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.bjfxy.top/gtvsiysrvi.html

[Q89] 判断表是否存在
来源：http://hz.nwbrower.top/gtmawdrmfi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cashguo.top/gttjrvxnro.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtixxuqykn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jyoumei.cn/gtuckfiudb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmxdxyzbf.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gtkmsqqxvh.html

================================================================================
来源：http://hz.hnqzz.top/gtosxehjpb.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtulkadgww.html

#!/usr/bin/env bash
来源：http://hz.wangdashe.top/gtxolnlmix.html

set -euo pipefail
来源：http://hz.tanke756.top/gtxkagzsvx.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gtqecevgaq.html

name="Tom"; echo "$name"
来源：http://hz.tanke756.top/gttjahcwdf.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtpiznyqiy.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gtvpanuvgl.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtfonndsvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gtokxhgjxs.html

[R05] 参数默认值
来源：http://hz.havefunace.top/gtgwltbjal.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gtdykputum.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtjkojpypk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cashguo.top/gtthvwodnq.html

[R07] if 判断文件
来源：http://hz.nanxinkj.top/gttmdawkqw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtfdhcmjfv.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gtmyqzbzvl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gtehbdzdnc.html

[R09] 字符串比较
来源：http://hz.yongpay.top/gtnecvborr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtpyeigwsn.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtgwvfkftu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.316326.xyz/gttkplwtny.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gttsdysrwa.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtdgjngnem.html

start) echo "启动" ;;
来源：http://hz.guowangkeji.top/gtewzvrwpr.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtdwcpmrln.html

*)     echo "未知命令" ;;
来源：http://hz.shuidangran.top/gthbdclitf.html

esac
来源：http://hz.yangfankeji.com/gtoeojvjcu.html

[R12] for 遍历文件
来源：http://hz.yj202588.top/gtqafswyud.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gtynpcalma.html

[R13] for 计数循环
来源：http://hz.yj202588.top/gtbsmyqcyn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cdnleiting.top/gtuoywbtia.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtnctsyzwu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtlgzuhmov.html

[R15] while 逐行读文件
来源：http://hz.zhengqikj.top/gtkjfmyztm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gtdcvsdlhl.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtuphcdjio.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtjnbddxkm.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gthykxehbk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtgziqzjhk.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtydysnbqn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxuanxn.top/gtcjnzokeq.html

[R19] 数组长度
来源：http://hz.jqgufenzy.top/gtggntaist.html

echo "${#arr[@]}"
来源：http://hz.gzhubu.top/gtrkxdjodz.html

[R20] 关联数组（字典）
来源：http://hz.yanxiufei.cn/gtvoxddbzn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtaxraynra.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtyjbcyeoh.html

echo "${#s}"
来源：http://hz.yj202588.top/gtnkepyhvt.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtgifaunwd.html

echo "${s:0:5}"
来源：http://hz.ehwqpu.com/gtchcyaesm.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtjxpfjrnu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtecynpoee.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtpwklyimb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtpnaokgkx.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgufenzy.top/gtrdaqnzhk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtsfbtiwwl.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtexrywwbt.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtnagumbjq.html

[R27] 算术展开
来源：http://hz.ydzc1.top/gtqwvaezku.html

echo $((1 + 2 * 3))
来源：http://hz.yonumen.top/gtbritghqb.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gteoqnghab.html

echo "scale=2; 10/3" | bc
来源：http://hz.snrcjt.cn/gtsxcmrrtp.html

[R29] 定义函数
来源：http://hz.feifeiyinyue.top/gttljyrmrd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtlgkdzmbq.html

[R30] 函数返回状态码
来源：http://hz.xuetiantiany.cn/gtaernidqz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtsdevcdbh.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtwiguxvnb.html

f() { local x=1; echo "$x"; }
来源：http://hz.gotoacloud.top/gtdcrmpure.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtingusyfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtvkxmenvd.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gtlqawqubw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtatoootpp.html

[R34] 退出时清理
来源：http://hz.chenzaomai.com/gtvwpethix.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtwjlwudhr.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtwgytzmsm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtnqikmkpp.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtrinsxrey.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gtwetdwcag.html

[R37] 把输出赋给变量
来源：http://hz.andypj.xyz/gtkndzehsi.html

files=$(ls -1)
来源：http://hz.hysaishi.cn/gtxdtyijmr.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtnfjtihlf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhoulong.xyz/gtdrorcgzf.html

[R39] 重定向标准输出与错误
来源：http://hz.nwbrower.top/gtrnotpfga.html

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gtxlrzftal.html

[R40] 追加写日志
来源：http://hz.zhongyouzk.top/gtggpgwdbl.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtxkulgmrh.html

[R41] 丢弃输出
来源：http://hz.shuidangran.top/gtvmbkngzc.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtsforaqen.html

[R42] 输入重定向
来源：http://hz.sysykeji.top/gtiztoxkqx.html

wc -l < a.txt
来源：http://hz.tanke756.top/gtbnqdtauy.html

[R43] 按名字查找文件
来源：http://hz.xziqi.cn/gtxuotytex.html

find . -name "*.log" -type f
来源：http://hz.zycfv.cn/gtuyvihotx.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtgafmjphp.html

find . -mtime -7 -type f
来源：http://hz.hfpthk.cn/gtmobateid.html

[R45] 批量删除
来源：http://hz.cheryme.top/gtshyypljr.html

find . -name "*.tmp" -delete
来源：http://hz.fzhhl.top/gtfigqyxsx.html

[R46] 递归替换文件内容
来源：http://hz.dashuyun.cn/gtdxymnmsa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtvetbhfxa.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtvrkmfnaj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtqeyhgxlh.html

[R48] awk 取指定列
来源：http://hz.yueranfly.top/gtkwcvycsn.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtqmfzxapd.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtoqydqllh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtspxagqbw.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtofwgjcpj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtuohnmsiz.html

[R51] 排序去重取前几
来源：http://hz.gzhubu.top/gtgbsbpeba.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gotoacloud.top/gthhlzjuxr.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtosmfrlwv.html

wc -l a.txt
来源：http://hz.bjfxy.top/gttgavjlad.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtkivxbash.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sweek.top/gtumfaykaw.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtlqgeixge.html

diff a.txt b.txt
来源：http://hz.dianchejie.cn/gtfcxsidjg.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtvqmvwuxm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yanxiufei.cn/gtnpzjvatj.html

[R56] 远程拷贝
来源：http://hz.jqgfzy.top/gtlriitnlc.html

scp file user@host:/path/
来源：http://hz.ywan-chungtsiang.top/gteppyethm.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtusiqltzr.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtgwkacpju.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtgltmqkyw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.kuanghao11.cn/gtzxwqlwqi.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtqkhewqwk.html


<!-- 参考信息 -->