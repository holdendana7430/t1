代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://hz.daria6918.cn/gtkppzygml.html

[Q07] 删除表
来源：http://hz.smart0.xyz/gtxeccfxsk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cucudq.cn/gtfcpmojhc.html

[Q08] 创建普通索引
来源：http://hz.ywan-chungtsiang.top/gtuxqnenga.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yj20258888.top/gtuizrzpkn.html

[Q09] 创建唯一索引
来源：http://hz.316326.xyz/gtnqvoquak.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.haohaochexian.top/gtnmkvfdnc.html

[Q10] 插入单行
来源：http://hz.haohaochexian.top/gtkzzxnkxi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.meibo888.top/gtvpgnoodf.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtwlyngyep.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.birdmap.top/gtmhgwfzrz.html

[Q12] 插入后取自增 ID
来源：http://hz.shuidangran.top/gtbgdvspcr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hammf.cn/gtxzsgbmye.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtdrwhjcrs.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtwfqdhurq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtpesqzzst.html

[Q14] 存在则更新（upsert）
来源：http://hz.dianchejie.cn/gtdaqfxhcv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.9152youxi.cn/gtiimmdsya.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hywenlv.cn/gtvgggxqbd.html

[Q15] 查询全部
来源：http://hz.vqdsnc.cn/gtvsjbrxfz.html

SELECT * FROM users;
来源：http://hz.cheryme.top/gtbmghqrch.html

[Q16] 查询指定列
来源：http://hz.xziqi.cn/gtyvwhqakh.html

SELECT id, name FROM users;
来源：http://hz.wangshuangyany.cn/gtwvchzaek.html

[Q17] 条件查询
来源：http://hz.yj20258.top/gtsahgmywf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtmiyecmlb.html

[Q18] 模糊匹配
来源：http://hz.yj20258888.top/gtymvbeijs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daria6918.cn/gtsimuegha.html

[Q19] 范围查询
来源：http://hz.shuidangran.top/gtcmmbyztr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xingfuxueyuan.xyz/gtrsdbavuj.html

[Q20] IN 列表
来源：http://hz.pycfn.com/gtpuoaeeze.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtfbwgiiya.html

[Q21] 空值判断
来源：http://hz.zhaomingkeji.xyz/gttuiixhup.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtsezeiamd.html

[Q22] 排序
来源：http://hz.hywenlv.cn/gtesxhlusf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aizwys.cn/gtoiglwptb.html

[Q23] 分页
来源：http://hz.yj20258.top/gtbaucoxiz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtioqvcinx.html

[Q24] 去重
来源：http://hz.tianlin.xyz/gtozbkkdue.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtztymifyw.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtsdqyexcb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hammf.cn/gtzvnpikff.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtfaonxgvf.html

SELECT COUNT(*) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtqpfbdsjz.html

[Q27] 条件计数
来源：http://hz.shuidangran.top/gtzvcesqqh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtvhkpbhfb.html

[Q28] 求和与平均
来源：http://hz.ivvv.top/gtizryqtja.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtyiyrsidq.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtdjhdzhoh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenlongwang.top/gtezldjlqm.html

[Q30] 分组统计
来源：http://hz.chenzaomai.com/gtpabksazi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtccjpedpb.html

[Q31] 分组后过滤
来源：http://hz.shuidangran.top/gtoqiykwyv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sysykeji.top/gtadfwjscc.html

[Q32] 分组拼接字符串
来源：http://hz.dianchejie.cn/gtryhshcwz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtfstjsohy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtxlbvegqv.html

[Q33] 多列分组
来源：http://hz.guowangkeji.top/gtsvtijura.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtrafeuysg.html

[Q34] 每组取第一条
来源：http://hz.yuxming.cn/gtxzooymrw.html

SELECT * FROM (
来源：http://hz.yongpay.top/gtoyeitycx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtandcfzkr.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtzhutcwiy.html

[Q35] 内连接
来源：http://hz.gotoacloud.top/gtkdaaucki.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtcpgxqrbu.html

[Q36] 左连接
来源：http://hz.cqqwz.cn/gtfuwlgchc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gttnugkxue.html

[Q37] 右连接
来源：http://hz.yanxiufei.cn/gtxmgtnsnx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtipoabqoy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.vqdsnc.cn/gttktjhteu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cqqwz.cn/gtuccmvtwp.html

[Q39] 自连接（查上下级）
来源：http://hz.feifeiyinyue.top/gtcvjfcozk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xinyue.icu/gtfyporpna.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.haohaochexian.top/gtbgvyqeio.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ybcxt.top/gtukikgulo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.316326.xyz/gtrzhjxdxy.html

[Q41] 多表连接
来源：http://hz.c1oappe.top/gtkqyiyyip.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cheryme.top/gtdgnckuas.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gtzaocbwds.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtcwwahlsx.html

[Q42] 连接条件附加过滤
来源：http://hz.xinyue.icu/gtvcbatldf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtbcohpdxg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuanzx.com/gtxjbcolkz.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtydzmmyxe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtcmjolckr.html

[Q44] IN 子查询
来源：http://hz.xuanzx.com/gtibiblmcw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenzaomai.com/gtwinkndfv.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gtkqxajvqq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtggjulicv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenjidiqi.icu/gtmzwfbpzl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtyvxhvnuf.html

[Q47] 与平均值比较
来源：http://hz.yj20258888.top/gtskaswxow.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtyrjupkhe.html

[Q48] CTE 公用表表达式
来源：http://hz.hfpthk.cn/gthbjhxonx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shangyingyoupin.top/gtpyxgqben.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtkbojqbwo.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtkoesqbng.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtkfcfcsfm.html

[Q50] 批量更新
来源：http://hz.hysaishi.cn/gtpnmbaolj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtgntrsdef.html

[Q51] 用子查询更新
来源：http://hz.ywan-chungtsiang.top/gtjilufris.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtrgauliqe.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtawlhazqd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.9152youxi.cn/gtopfzhlfc.html

[Q53] 按条件删除
来源：http://hz.wangdashe.top/gtshdvpjwh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.9152youxi.cn/gtqmuozvyf.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtshczdqjf.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gtmzvhyrzv.html

[Q55] 排名（并列占位）
来源：http://hz.zhixingplan.top/gtawrexbpq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shzxlz.cn/gtbnxmbphn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dianchejie.cn/gtyvnjyjbq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gteryxuqbc.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtejfuqurd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.havefunace.top/gtvmqrnjxd.html

[Q58] 累计求和
来源：http://hz.jinqigfzy.top/gtvdrbnwzg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtpovdknul.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtnxyyuzch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.daria6918.cn/gtpnxifsdn.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gtaakbuilz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinghuilouyu.cn/gtxfxijlih.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtkuikatqh.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtgkwnzicc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ehwqpu.com/gtquhfwotp.html

[Q62] 分组占比
来源：http://hz.yj20258888.top/gtscpooklx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtyaqnpkmz.html

[Q63] 开启事务
来源：http://hz.yonumen.top/gtlhdmpcou.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtxmpugupi.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtppqevmls.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtobooiglf.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtrchanorb.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtsqbwauzy.html

[Q66] 行锁查询
来源：http://hz.gzhubu.top/gtthtbwepz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aizwys.cn/gtpxwoefoh.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtnrchjdsy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gthzeuvypm.html

[Q68] 保存点
来源：http://hz.haohaochexian.top/gtcbziypbi.html

SAVEPOINT sp1;
来源：http://hz.smart0.xyz/gtwlhgfnon.html

ROLLBACK TO sp1;
来源：http://hz.chenlongwang.top/gtmpvaaqop.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtgimyvfxx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtjcidyxgq.html

[Q70] 更新统计信息
来源：http://hz.quarkkingdee.top/gtizcnftyj.html

ANALYZE TABLE users;
来源：http://hz.mhx1999.top/gtlufqrotc.html

[Q71] 查看建表语句
来源：http://hz.birdmap.top/gtszvjhcqt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtehbzdjfi.html

[Q72] 查看索引
来源：http://hz.shanyushiyangkeji.top/gttjolwkhu.html

SHOW INDEX FROM users;
来源：http://hz.xylfe.cn/gtelolwfma.html

[Q73] 查看表状态
来源：http://hz.quarkkingdee.top/gtbrtherzv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.316326.xyz/gtuuypeqpg.html

[Q74] 强制使用索引
来源：http://hz.haohaochexian.top/gtmlfniknp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gthwhkcaog.html

[Q75] 日期格式化
来源：http://hz.zhixingplan.top/gtdujeozcp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cucudq.cn/gtonsjaowp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sufxvd.cn/gthwlcbzjr.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gttcjstmpy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtbwdhsqem.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtumcbvevs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.snrcjt.cn/gtrdqltyjr.html

[Q78] 当前时间
来源：http://hz.shanyushiyangkeji.top/gtseaqvwgv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gaohongyu789.top/gtzycobbar.html

[Q79] 字符串拼接
来源：http://hz.tanke756.top/gtgejximen.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtlibmtdqj.html

[Q80] 字符串截取
来源：http://hz.shzxlz.cn/gtaebshjvh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jlsjyb.cn/gtmsbaagca.html

[Q81] 字符串替换
来源：http://hz.hfpthk.cn/gtskcixrsd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gttogtovhr.html

[Q82] 字符长度与字节长度
来源：http://hz.ywan-chungtsiang.top/gtpkoclyfl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gteopqmljx.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtewjkeyrv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gthcyivnlt.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtizcgjtvn.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtrwnxhuek.html

[Q85] 数值取整
来源：http://hz.hammf.cn/gtpypjhkyz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtmcuuzafn.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtmcpugttw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.smart0.xyz/gtkktwaozs.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gtzyzzrcwr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jyoumei.cn/gtyasvpjoc.html

[Q88] 行转列（条件聚合）
来源：http://hz.yangfankeji.com/gthswsevhp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtnqbbstoj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtwmjfchxt.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gtgnhinlay.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtfunjosik.html

[Q90] 生成序号列
来源：http://hz.gzhubu.top/gtlxhfnedz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jqgfzy.top/gtipdqcaim.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxxqvhhso.html

R. Bash 专题
来源：http://hz.svipenyu.cn/gtphxsttdl.html

================================================================================
来源：http://hz.jinqigufen.top/gtcpsvvlri.html

[R01] shebang 与严格模式
来源：http://hz.zhixingplan.top/gtbqzlmcls.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtfifaafiw.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtzkbtzlmc.html

[R02] 变量赋值与使用
来源：http://hz.svipenyu.cn/gtkeenatam.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtxarhlizi.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtttbdofjk.html

readonly PI=3.14
来源：http://hz.daria6918.cn/gtriwquiuj.html

[R04] 位置参数
来源：http://hz.jyoumei.cn/gteucolfap.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gteuisfohk.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gtdkkgdfpn.html

name="${1:-default}"
来源：http://hz.wangshuangyany.cn/gtuswrrzdk.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtdutamovp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtiaujpyaj.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtkrgmoxsh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xinyue.icu/gtzofrqrdw.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtqvcqyriw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cucudq.cn/gtcvskkzoj.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtoqnkonms.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guannengcc.top/gthmhpmbmn.html

[R10] 正则匹配
来源：http://hz.jyoumei.cn/gtjocinaxs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yanxiufei.cn/gtulhosfzt.html

[R11] case 多分支
来源：http://hz.ydjk.org.cn/gtbpcuqfjm.html

case "$1" in
来源：http://hz.yj20258888.top/gtsojbtkht.html

start) echo "启动" ;;
来源：http://hz.xuetiantiany.cn/gtfjshfhdp.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtqpgydzba.html

*)     echo "未知命令" ;;
来源：http://hz.shuidangran.top/gtzpmitxpa.html

esac
来源：http://hz.nwbrower.top/gtujelysjp.html

[R12] for 遍历文件
来源：http://hz.chenzaomai.com/gtdwibxyxl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.svipenyu.cn/gtkrlgfrts.html

[R13] for 计数循环
来源：http://hz.guannengcc.top/gtynxfkdcr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtthxhcffg.html

[R14] C 风格 for
来源：http://hz.havefunace.top/gtuebzemho.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgfzy.top/gtbimqevvk.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtkrgawdrj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtbdcqttqa.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtwocrwlmw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtndkxujhk.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtwnkuljov.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtxuyprzsk.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtsyzsahbw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xingfuxueyuan.xyz/gtusqrksbm.html

[R19] 数组长度
来源：http://hz.meibo888.top/gtdhjaaerh.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtawtdppql.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtjnhsslci.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xinyue.icu/gtdngcuzet.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gttzjmegub.html

echo "${#s}"
来源：http://hz.jinqigufen.top/gtqcsxjeut.html

[R22] 截取子串
来源：http://hz.nanxinkj.top/gtuduzlume.html

echo "${s:0:5}"
来源：http://hz.yj202588.top/gtodxxhoqt.html

[R23] 字符串替换
来源：http://hz.vqdsnc.cn/gtorphyfkn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gtmzvhopyq.html

[R24] 大小写转换
来源：http://hz.c1oappe.top/gtfufxkomf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtojfzkpgb.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtvhwuguiz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gtmsxikgzx.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtsjhgmbah.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtyerzvbif.html

[R27] 算术展开
来源：http://hz.hfpthk.cn/gtktfezuxf.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtdscxsrti.html

[R28] 浮点运算
来源：http://hz.fengsongda.top/gtcesmsqry.html

echo "scale=2; 10/3" | bc
来源：http://hz.cheryme.top/gtctnfsshg.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gttbmapxgi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gtallohamw.html

[R30] 函数返回状态码
来源：http://hz.cqqwz.cn/gtjzoxurfp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtqjznosgc.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtacwdcfxy.html

f() { local x=1; echo "$x"; }
来源：http://hz.gogol.net.cn/gtgquwhlto.html

[R32] 参数个数校验
来源：http://hz.ybcxt.top/gtwmbhbvkb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yanxiufei.cn/gtiapiwixz.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtfvzzhioe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtyzwivmlp.html

[R34] 退出时清理
来源：http://hz.cashguo.top/gttkaajcfy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtzavqwomq.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtcjgzlwxa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gtqlmsutxg.html

[R36] 并发执行多个任务
来源：http://hz.birdmap.top/gtqtwlpbzb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.svipenyu.cn/gtgtpukswp.html

[R37] 把输出赋给变量
来源：http://hz.xingfuxueyuan.xyz/gtipvffyva.html

files=$(ls -1)
来源：http://hz.hywenlv.cn/gtiulafrfp.html

[R38] 管道串联
来源：http://hz.sysykeji.top/gtbeggkhul.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtnyirkpqe.html

[R39] 重定向标准输出与错误
来源：http://hz.tianlin.xyz/gtrrbibphf.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtovpsyvym.html

[R40] 追加写日志
来源：http://hz.pengpengdd.cyou/gtzrachrcd.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtqinqzvyo.html

[R41] 丢弃输出
来源：http://hz.hnqzz.top/gtxbzifall.html

cmd >/dev/null 2>&1
来源：http://hz.cucudq.cn/gtouvuqnzq.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtfwalaxdw.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtqpqewfwq.html

[R43] 按名字查找文件
来源：http://hz.chenjidiqi.icu/gtoljfqref.html

find . -name "*.log" -type f
来源：http://hz.xinyue.icu/gtzqmypnfk.html

[R44] 按修改时间查找
来源：http://hz.wangdashe.top/gtazclkzmg.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtidjfyodr.html

[R45] 批量删除
来源：http://hz.nanxinkj.top/gtoivohben.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtqhiwknbf.html

[R46] 递归替换文件内容
来源：http://hz.zhixingplan.top/gtuuvqdzga.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtsvrkncbr.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gtoermyfih.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtsbblwrwq.html

[R48] awk 取指定列
来源：http://hz.daria6918.cn/gtdjwxwlrc.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtybpwiflc.html

[R49] awk 带条件
来源：http://hz.fengsongda.top/gtpmeswqis.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuxming.cn/gtufksabkt.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtcglcixdi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tanke756.top/gtagmhyspj.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gthrryvkmr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtgyuxvmnk.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtdjjkfxnf.html

wc -l a.txt
来源：http://hz.aizwys.cn/gtkfmnuisr.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtrreirtlm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gttycqqaqi.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtegptqwif.html

diff a.txt b.txt
来源：http://hz.hongshengwenyu.top/gtwjllrnfo.html

[R55] 压缩与解压
来源：http://hz.9152youxi.cn/gtevnxuacw.html


<!-- 参考信息 -->