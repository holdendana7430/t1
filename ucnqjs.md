代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cashguo.top/gtvoriwhng.html

[Q09] 创建唯一索引
来源：http://hz.havefunace.top/gtnroljzvs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hywenlv.cn/gtbbkqqpce.html

[Q10] 插入单行
来源：http://hz.fzhhl.top/gtidgnavrr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtkrmhtdwv.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gtfxeegrbk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hysaishi.cn/gttzvdwbfp.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtwrinplhe.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenjidiqi.icu/gtvgmlxqgz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenjidiqi.icu/gtaawdjasj.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtoalffcdt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhaomingkeji.xyz/gtjcgrhjla.html

[Q14] 存在则更新（upsert）
来源：http://hz.pycfn.com/gtpqwjeaae.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gtusueejvt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhiwuduotai.top/gtdgzafwnp.html

[Q15] 查询全部
来源：http://hz.zhiwuduotai.top/gtegpwnoov.html

SELECT * FROM users;
来源：http://hz.jinqigfzy.top/gtbpgmlnrk.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtnyxxcgim.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtehyzbvuw.html

[Q17] 条件查询
来源：http://hz.yj20258888.top/gtbbsmwwvp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtboulbymc.html

[Q18] 模糊匹配
来源：http://hz.ppjwa.cn/gthsqhwqtq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xinyue.icu/gtnjveswxr.html

[Q19] 范围查询
来源：http://hz.iojbl.cn/gtetfihvzo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtypskfpzp.html

[Q20] IN 列表
来源：http://hz.nanxinkj.top/gthfzfigty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhaomingkeji.xyz/gtpypgkrln.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gtdcewvamp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hfpthk.cn/gttxzglkji.html

[Q22] 排序
来源：http://hz.gogol.net.cn/gteqdlscol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.cdnleiting.top/gtrnfhlhlg.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtoiqfxhtg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jlsjyb.cn/gtqxbermqg.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtbwcfvlvo.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtdbxxwpcd.html

[Q25] 只取前 N 条
来源：http://hz.xuanzx.com/gtyqoxqtpa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtoqpolttw.html

[Q26] 计数
来源：http://hz.jiagoushi.top/gtumgfisah.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtwplagwpg.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtisgaebpq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fengsongda.top/gtlgutgvnv.html

[Q28] 求和与平均
来源：http://hz.ppjwa.cn/gtdbgyhuvj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yvedp.cn/gtenijrwcs.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gtwddlfnnd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtlwpesyrj.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtqvvfliaq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtwvqawnco.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtwaasichp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yangfankeji.com/gtydiejxvl.html

[Q32] 分组拼接字符串
来源：http://hz.0kj1m.cn/gtojzrjhya.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtgqbdabvp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtyamioyvc.html

[Q33] 多列分组
来源：http://hz.yongpay.top/gtsmigsmth.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xuetiantiany.cn/gthclzsjrr.html

[Q34] 每组取第一条
来源：http://hz.jiagoushi.top/gtutzrbhjs.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gtzoaxmblz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xylfe.cn/gtvqpxdvql.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtcwxvkykt.html

[Q35] 内连接
来源：http://hz.shanyushiyangtech.top/gtlnbkhoxy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgfzy.top/gtemuusfsj.html

[Q36] 左连接
来源：http://hz.snrcjt.cn/gtvlxlqdqh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtzaijjtqq.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gtqvdvureq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnxiangtu.top/gtnbseuhnb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daria6918.cn/gtnfhpaclj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gtmmtvduzm.html

[Q39] 自连接（查上下级）
来源：http://hz.cheryme.top/gtdfkgszgi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtmcsuljgt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinyuanbaomall.cn/gtqvqnlkin.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tian-w.cn/gtpwohrwtr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daxiang520.top/gtaoqnrcem.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtzzolcgnu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gotoacloud.top/gtobloqatm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhengqikj.top/gtygiaadkw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gtdxbcotgo.html

[Q42] 连接条件附加过滤
来源：http://hz.hnxiangtu.top/gtebpjeoxu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yvedp.cn/gthqgwxwpn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtodtlbbtr.html

[Q43] 标量子查询
来源：http://hz.sufxvd.cn/gtddxegjtg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jlsjyb.cn/gtzlywbzmd.html

[Q44] IN 子查询
来源：http://hz.hammf.cn/gtdyoyplki.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yangfankeji.com/gtwkkxshvj.html

[Q45] EXISTS 判断存在
来源：http://hz.gaohongyu789.top/gtcwegemrm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtdqxcmckr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.feifeiyinyue.top/gtwnccqzed.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtbsjttdln.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtmathchcw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.bjfxy.top/gtupeccawo.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gttrfcfump.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gtllpuuvzt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gogol.net.cn/gtvaljatli.html

[Q49] 更新单行
来源：http://hz.pengpengdd.cyou/gtnhwhhuvu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jiagoushi.top/gtzsletnnj.html

[Q50] 批量更新
来源：http://hz.sweek.top/gtklbkoobq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhiwuduotai.top/gtwjzqyidb.html

[Q51] 用子查询更新
来源：http://hz.daria6918.cn/gtvkvgefgm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yanxiufei.cn/gtwcgcwihe.html

[Q52] 删除指定行
来源：http://hz.daxiang520.top/gttnnpulbr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhengqikj.top/gtoyfzrzuy.html

[Q53] 按条件删除
来源：http://hz.tianlin.xyz/gtrqbulrur.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtfvrslicb.html

[Q54] 清空表
来源：http://hz.c1oappe.top/gtbtberdim.html

TRUNCATE TABLE logs;
来源：http://hz.zhiwuduotai.top/gtecdvxdtu.html

[Q55] 排名（并列占位）
来源：http://hz.yvedp.cn/gtwklldghs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhixingplan.top/gthmvycbko.html

[Q56] 密集排名（并列不占位）
来源：http://hz.snrcjt.cn/gtbkwfuarj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fengsongda.top/gtjuktiqaf.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gthwbcsylp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xylfe.cn/gtlttvqtah.html

[Q58] 累计求和
来源：http://hz.yongpay.top/gtckiepibt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtofzporsw.html

[Q59] 分组内累计
来源：http://hz.guannengcc.top/gtkmcjrosq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtnjzqojck.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtnwjpztfv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtqyofdcwp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtucsthazt.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gtvtyuisdx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtopqudcla.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gthzpyfwjx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtkppryats.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gtuwnmwjfk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtcpeelkov.html

[Q64] 提交事务
来源：http://hz.sufxvd.cn/gtqcrvypmn.html

COMMIT;
来源：http://hz.ehwqpu.com/gtnguabtuh.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtxhyyeeih.html

ROLLBACK;
来源：http://hz.jinqigufen.top/gtqtcdzwja.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtmfleimcx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuxming.cn/gtltvlkrft.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtfyakkzlr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tianlin.xyz/gtymgtpckk.html

[Q68] 保存点
来源：http://hz.yj20258.top/gtrzyifike.html

SAVEPOINT sp1;
来源：http://hz.jinyuanbaomall.cn/gtbdzgapul.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gtalqmdmgq.html

[Q69] 查看执行计划
来源：http://hz.316326.xyz/gtwqejobzn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtbhplprmc.html

[Q70] 更新统计信息
来源：http://hz.daxiang520.top/gtcdnbgggn.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtjccntsfc.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtowcahzuh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtgcszdxpe.html

[Q72] 查看索引
来源：http://hz.kuanghao11.cn/gtemfcokqn.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtrzpvrvsu.html

[Q73] 查看表状态
来源：http://hz.ybcxt.top/gtsjekraln.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.redwolf501.top/gtdcrrdgmi.html

[Q74] 强制使用索引
来源：http://hz.chenlongwang.top/gtuhgoqonl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinyuanbaomall.cn/gtqelyrjjt.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtuctjrpqj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtzhwltgcy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ppjwa.cn/gtstzggxlb.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtattnmtoo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhiwuduotai.top/gtaksuvjsc.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtqatvmabh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhaomingkeji.xyz/gtbqtlyebc.html

[Q78] 当前时间
来源：http://hz.daxiang520.top/gtrwafquef.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtvelzdrcl.html

[Q79] 字符串拼接
来源：http://hz.yonumen.top/gtjdofxthf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daria6918.cn/gtsxjjtqca.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtplvveopj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jiagoushi.top/gtutohycvg.html

[Q81] 字符串替换
来源：http://hz.andypj.xyz/gtpvpjxttt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtvkardowe.html

[Q82] 字符长度与字节长度
来源：http://hz.ybcxt.top/gterqrdkvj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258888.top/gtzngtswhh.html

[Q83] 大小写转换
来源：http://hz.guannengcc.top/gthygehbqg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtfopdkrbv.html

[Q84] 去除首尾空格
来源：http://hz.hammf.cn/gtahimnkhr.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtfjpkybhu.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtmilmvxrv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhiwuduotai.top/gtczfzeonq.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtjkonzgzv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gtcmjdyzrs.html

[Q87] JSON 字段做条件
来源：http://hz.gotoacloud.top/gtmmdjhcxe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yanxiufei.cn/gtuefzqgtz.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxuanxn.top/gthkawdhad.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yueranfly.top/gtblkhdurb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tian-w.cn/gtmsmyltae.html

[Q89] 判断表是否存在
来源：http://hz.sysykeji.top/gtrukronwl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtsmajtsvc.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtbpjduyqc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtzniwqrgk.html

================================================================================
来源：http://hz.zhengqikj.top/gtkrqnbgsr.html

R. Bash 专题
来源：http://hz.yj20258.top/gtdjbbgbxq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gteikorfve.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtzpmyxjzm.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtrsdvrfam.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtjbkkxwqj.html

[R02] 变量赋值与使用
来源：http://hz.cheryme.top/gtqfqkeype.html

name="Tom"; echo "$name"
来源：http://hz.316326.xyz/gtnouzjdwy.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtgncskcgy.html

readonly PI=3.14
来源：http://hz.yonumen.top/gtlariruls.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gthfkdbytf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtbytqbhyl.html

[R05] 参数默认值
来源：http://hz.sweek.top/gtexlpsgmv.html

name="${1:-default}"
来源：http://hz.hongshengwenyu.top/gtonqcfjbi.html

[R06] 判断命令是否存在
来源：http://hz.gogol.net.cn/gtxtiadglu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.mhx1999.top/gtykbxksgk.html

[R07] if 判断文件
来源：http://hz.jianghu66.top/gtmwapnhcn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gthbdvpepe.html

[R08] 数值比较
来源：http://hz.jinyuanbaomall.cn/gtbzyaatkj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gtdejqrhgc.html

[R09] 字符串比较
来源：http://hz.kuanghao11.cn/gtouodwbzd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxuanxn.top/gtqkhscjzi.html

[R10] 正则匹配
来源：http://hz.9152youxi.cn/gteipcmiui.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fzhhl.top/gttfibmmfo.html

[R11] case 多分支
来源：http://hz.yanxiufei.cn/gtybhimvbh.html

case "$1" in
来源：http://hz.sweek.top/gtywaskruy.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtbyviirwk.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtolslquyi.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gthkandadd.html

esac
来源：http://hz.yj20258.top/gtzwwbcgva.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtpxlqzlgl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtaxsvprxf.html

[R13] for 计数循环
来源：http://hz.jqgfzy.top/gtxlebuuck.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hammf.cn/gtdqxxhfgz.html

[R14] C 风格 for
来源：http://hz.xylfe.cn/gtkxysgnob.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtcphoipui.html

[R15] while 逐行读文件
来源：http://hz.yonumen.top/gttslkzghf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.pengpengdd.cyou/gtwgawreyh.html

[R16] until 等待条件
来源：http://hz.nwbrower.top/gtoxywvprt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hfpthk.cn/gtedujtffm.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtjqoqmesg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cqqwz.cn/gtckxabisz.html

[R18] 遍历数组
来源：http://hz.andypj.xyz/gtbfaerami.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cheryme.top/gtpocwgodj.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtzvcqcjrc.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtximkcciz.html

[R20] 关联数组（字典）
来源：http://hz.gaohongyu789.top/gtuheiikmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhoulong.xyz/gtzshyuutw.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtdsknajrr.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtbfjsbasr.html

[R22] 截取子串
来源：http://hz.quarkkingdee.top/gtwcutlqet.html

echo "${s:0:5}"
来源：http://hz.cheryme.top/gtwbpghevf.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtkpkyxiuu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yvedp.cn/gtfxegfuon.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtcwdhlfqi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ppjwa.cn/gtgbmveqef.html

[R25] 去后缀 / 去前缀
来源：http://hz.gzhubu.top/gtfbmbuzyv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.quarkkingdee.top/gtdudgfcdl.html

[R26] 命令替换
来源：http://hz.hnqzz.top/gtohaadeqx.html

now=$(date +%F); echo "$now"
来源：http://hz.zhaomingkeji.xyz/gtjixdafnx.html

[R27] 算术展开
来源：http://hz.birdmap.top/gtypfzfbgw.html

echo $((1 + 2 * 3))
来源：http://hz.snrcjt.cn/gtwotnvsna.html

[R28] 浮点运算
来源：http://hz.zhoulong.xyz/gtpsfffcyo.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtrdkkpvej.html

[R29] 定义函数
来源：http://hz.hywenlv.cn/gtgqutlbxj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yvedp.cn/gtqhmvyqsx.html

[R30] 函数返回状态码
来源：http://hz.yj20258888.top/gtqvxmhjho.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jlsjyb.cn/gtswxtqwvn.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtttubpyvh.html

f() { local x=1; echo "$x"; }
来源：http://hz.xuetiantiany.cn/gtvrdkvaph.html

[R32] 参数个数校验
来源：http://hz.jiagoushi.top/gthgauynlr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gtzyiyamrz.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtrmqtjekh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtmddzgtvx.html

[R34] 退出时清理
来源：http://hz.gzhubu.top/gtmpubcaht.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtbaclhdst.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangtech.top/gtqhmqsxui.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtxuiawacl.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangkeji.top/gtwrrtolcz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtjjoxqkvc.html

[R37] 把输出赋给变量
来源：http://hz.hfpthk.cn/gtvjlwcqqe.html

files=$(ls -1)
来源：http://hz.redwolf501.top/gtwelppxur.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtggvhprem.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gttjrwwqrw.html

[R39] 重定向标准输出与错误
来源：http://hz.sysykeji.top/gtlafdabck.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtarnjsdlr.html

[R40] 追加写日志
来源：http://hz.cdnleiting.top/gtorbszxev.html

echo "log" >> out.log
来源：http://hz.yj20258888.top/gtfufnwggb.html

[R41] 丢弃输出
来源：http://hz.zhoulong.xyz/gtxeyaubjg.html

cmd >/dev/null 2>&1
来源：http://hz.jqgufenzy.top/gtjqladdtm.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gtbubmotte.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtdqkfhzuz.html

[R43] 按名字查找文件
来源：http://hz.xziqi.cn/gtajmfvzcd.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtikwmmxcx.html

[R44] 按修改时间查找
来源：http://hz.redwolf501.top/gthpaqnvuw.html

find . -mtime -7 -type f
来源：http://hz.jinghuilouyu.cn/gtsnyewdbh.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtfhcfcdyi.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtwvvfsnsq.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtgnkhrxhs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtdnsebckx.html

[R47] sed 单行替换
来源：http://hz.fzhhl.top/gtwfldbdks.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtjfybzmua.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gtrgaltpul.html

awk '{print $1, $3}' a.txt
来源：http://hz.gotoacloud.top/gtddqusdwt.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtupqoocey.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtnymahnec.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtpfwycigl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gthxeyujrj.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtaanmduvl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtzxzjjplw.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtfwqhewhb.html

wc -l a.txt
来源：http://hz.yongpay.top/gthbdphjja.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtcgkkgnal.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gtbtyvwpve.html

[R54] 比较两个文件
来源：http://hz.hysaishi.cn/gtxlfeyriz.html

diff a.txt b.txt
来源：http://hz.redwolf501.top/gtgsytpyoy.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtrcbrqrbo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtibuvyzgc.html

[R56] 远程拷贝
来源：http://hz.jinyuanbaomall.cn/gtieiqdujy.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtbnvlnxrj.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtqkpixxgu.html


<!-- 参考信息 -->