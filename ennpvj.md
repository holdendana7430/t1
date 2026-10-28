代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtdcooccpl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tanke756.top/gtkwqmsxep.html

[Q13] 忽略重复插入
来源：http://hz.cashguo.top/gtnqgovsqv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtdlxqweho.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtzgrajzdf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yanxiufei.cn/gtibmnvdvn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.9152youxi.cn/gtwickvrqt.html

[Q15] 查询全部
来源：http://hz.nanxuanxn.top/gtnryozzvq.html

SELECT * FROM users;
来源：http://hz.shangyingyoupin.top/gtjvwzypbx.html

[Q16] 查询指定列
来源：http://hz.guannengcc.top/gtecevfqya.html

SELECT id, name FROM users;
来源：http://hz.nwbrower.top/gtnwwlcxvv.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtzqlnbbgy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gtqghxkyqm.html

[Q18] 模糊匹配
来源：http://hz.cheryme.top/gtetzytltf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.aizwys.cn/gtfyfzwoqa.html

[Q19] 范围查询
来源：http://hz.sysykeji.top/gthayxnqin.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.havefunace.top/gtuyvolxju.html

[Q20] IN 列表
来源：http://hz.yonumen.top/gtvhdkigkr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtfeezeqfc.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gteyrozlda.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhaomingkeji.xyz/gtbxdtupgt.html

[Q22] 排序
来源：http://hz.316326.xyz/gtenswhhfj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.snrcjt.cn/gtmvgpubsa.html

[Q23] 分页
来源：http://hz.yj20258.top/gtecarqgno.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtqqiyqgey.html

[Q24] 去重
来源：http://hz.cashguo.top/gttjliuatb.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gthzonwihn.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtgozidlgj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtwxufqdkz.html

[Q26] 计数
来源：http://hz.cheryme.top/gtsmpjiicz.html

SELECT COUNT(*) FROM users;
来源：http://hz.hongshengwenyu.top/gtmvugiwpx.html

[Q27] 条件计数
来源：http://hz.ppjwa.cn/gtjpcmxzfa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fengsongda.top/gtjzsujyru.html

[Q28] 求和与平均
来源：http://hz.feifeiyinyue.top/gtcavfziwh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtgjdmaqld.html

[Q29] 最大最小值
来源：http://hz.zdqjudy.top/gtczciypzk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtkezeymxr.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gtidhwjkpp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtaqbyosdb.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gttvxvymcf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yonumen.top/gtvpmymuvo.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtpoewfhgc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtozbvtzjq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgfzy.top/gthtsafvqn.html

[Q33] 多列分组
来源：http://hz.kuanghao11.cn/gtsaeunohd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cucudq.cn/gtrxlptqra.html

[Q34] 每组取第一条
来源：http://hz.gogol.net.cn/gtsjwychcc.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gthjuvbzdu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtkojknljh.html

) t WHERE rn = 1;
来源：http://hz.bjfxy.top/gtfpxewuyz.html

[Q35] 内连接
来源：http://hz.chenzaomai.com/gtyzkulhzr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtqczoknal.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gtpuxixghc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtgfssuhvj.html

[Q37] 右连接
来源：http://hz.cdnleiting.top/gtmghvbcxp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zdqjudy.top/gtwndhkfev.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.snrcjt.cn/gtureatbyv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinghuilouyu.cn/gtzjgmmrlg.html

[Q39] 自连接（查上下级）
来源：http://hz.sysykeji.top/gtumvulwwx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gzhubu.top/gtskggqjkd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtoomlunqf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dashuyun.cn/gtoqmigtik.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tianlin.xyz/gtdbpgiolj.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtikdwunxf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gttlgbocuv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.mhx1999.top/gtxwomcptg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tianlin.xyz/gtydmkqkcr.html

[Q42] 连接条件附加过滤
来源：http://hz.ehwqpu.com/gtrlkkltzm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cqqwz.cn/gtwxymjhoe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aizwys.cn/gtweokwfjo.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtscfotcee.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtkmwpbfxw.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtvjwxyipq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guowangkeji.top/gteqcpfehc.html

[Q45] EXISTS 判断存在
来源：http://hz.nwbrower.top/gtqantoohz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gttxpkgtje.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtppgnvmxm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtmhsbyini.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtzrqiwsrv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fzhhl.top/gtdhigrxee.html

[Q48] CTE 公用表表达式
来源：http://hz.wangshuangyany.cn/gtifuwhjdg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hywenlv.cn/gtqigkdpdo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhongyouzk.top/gtyqmuwzni.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtejwnuyby.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.bjfxy.top/gtodfupbuu.html

[Q50] 批量更新
来源：http://hz.yj202588.top/gtftwyttbf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhengqikj.top/gtajhcubop.html

[Q51] 用子查询更新
来源：http://hz.hywenlv.cn/gtygaefrqj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gttpuqwsul.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtjffwogjp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sweek.top/gtxqnskiym.html

[Q53] 按条件删除
来源：http://hz.pycfn.com/gtuarcqztd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtztknmtli.html

[Q54] 清空表
来源：http://hz.xuetiantiany.cn/gtmrofgudn.html

TRUNCATE TABLE logs;
来源：http://hz.jqgfzy.top/gtrjpgrkok.html

[Q55] 排名（并列占位）
来源：http://hz.yongpay.top/gtskwvgrbz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.svipenyu.cn/gtkvihkdvz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.52xcode.cn/gtwkpjbznk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhoulong.xyz/gtfutvwzpp.html

[Q57] 行号
来源：http://hz.52xcode.cn/gttlvlgjex.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gtdzmxxzib.html

[Q58] 累计求和
来源：http://hz.yuxming.cn/gtfwnjgquy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtlawwmczi.html

[Q59] 分组内累计
来源：http://hz.pengpengdd.cyou/gtvnoezvub.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgfzy.top/gtbnjyoduk.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gtjkrvxdrw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtcqjchqhd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtsohfmlga.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtfowhvskh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtpbxxchxq.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gttjqqhhnh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtlbvbjwnh.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtbfmgovea.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtrrjrdews.html

[Q64] 提交事务
来源：http://hz.feifeiyinyue.top/gtwtjegllo.html

COMMIT;
来源：http://hz.c1oappe.top/gtprzlmzze.html

[Q65] 回滚事务
来源：http://hz.yj20258.top/gtxxznvhwo.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtbxqnlzfh.html

[Q66] 行锁查询
来源：http://hz.hysaishi.cn/gtiakwlcet.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gtkchnkcxg.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtjpvwtpns.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gotoacloud.top/gtlufztitz.html

[Q68] 保存点
来源：http://hz.feifeiyinyue.top/gtpierehpk.html

SAVEPOINT sp1;
来源：http://hz.sweek.top/gtgigqjgyw.html

ROLLBACK TO sp1;
来源：http://hz.hnxiangtu.top/gthjmvrhak.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtvyvblwun.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtobwivzjj.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtolsdpfbl.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtadkxutwc.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtrfegnbis.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuxming.cn/gtfmjzgajm.html

[Q72] 查看索引
来源：http://hz.snrcjt.cn/gtgjxkfaub.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtldqwcoai.html

[Q73] 查看表状态
来源：http://hz.birdmap.top/gtklqmbxph.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aizwys.cn/gtwxwoocpt.html

[Q74] 强制使用索引
来源：http://hz.nanxuanxn.top/gtqwexxoat.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ywan-chungtsiang.top/gtdnytdgdc.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtelhxoxbg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.smart0.xyz/gtaqszkhob.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhengqikj.top/gttgdovcco.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtoyhaxqib.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aizwys.cn/gtloizxowu.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gtcopujzua.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtpddkwxtq.html

[Q78] 当前时间
来源：http://hz.9152youxi.cn/gtukawtzmu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtxgxynzca.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtyqjnvfot.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenlongwang.top/gtecqggctu.html

[Q80] 字符串截取
来源：http://hz.nanxuanxn.top/gtftgbkybk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtjpqyveoe.html

[Q81] 字符串替换
来源：http://hz.wangshuangyany.cn/gtfnejwiam.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ybcxt.top/gtvtzjgwdg.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtuczaruhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sufxvd.cn/gttzbctxfv.html

[Q83] 大小写转换
来源：http://hz.mhx1999.top/gtcbckamoe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daxiang520.top/gtxueymcww.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gthfmhulex.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtfxdhmtrp.html

[Q85] 数值取整
来源：http://hz.c1oappe.top/gtpdhfvjuq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtweawbhcm.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtqwzqayng.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtxaniendr.html

[Q87] JSON 字段做条件
来源：http://hz.pycfn.com/gtubhgkzgc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yuxming.cn/gtkxbpnygm.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnxiangtu.top/gtdkceicqo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xylfe.cn/gtzxcnhbkk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtwjmvcywg.html

[Q89] 判断表是否存在
来源：http://hz.zycfv.cn/gtvdrfcebe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.9152youxi.cn/gtnukmqzik.html

[Q90] 生成序号列
来源：http://hz.jiagoushi.top/gtnoizrtjh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtgvmvuris.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtfdksfynp.html

R. Bash 专题
来源：http://hz.shangyingyoupin.top/gthbldgdxu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzekpzpev.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtapomztnb.html

#!/usr/bin/env bash
来源：http://hz.daria6918.cn/gtxvkjbrdi.html

set -euo pipefail
来源：http://hz.yangfankeji.com/gtmgqrxaed.html

[R02] 变量赋值与使用
来源：http://hz.hnxiangtu.top/gtqospuqhy.html

name="Tom"; echo "$name"
来源：http://hz.hnxiangtu.top/gttxozrnhe.html

[R03] 只读变量
来源：http://hz.guannengcc.top/gtappqlwwn.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtrixrnwiv.html

[R04] 位置参数
来源：http://hz.jiagoushi.top/gtrbetzfck.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gthlugkdnw.html

[R05] 参数默认值
来源：http://hz.cqqwz.cn/gtsbqmvmhx.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtdwmrswcw.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gthjjgtahs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtaoisxynj.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtoaopprly.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtgcqswkld.html

[R08] 数值比较
来源：http://hz.sxryk.cn/gtqlimvwie.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nanxuanxn.top/gtfscakzwe.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gthoojygxc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dashuyun.cn/gtaqncxram.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtudrlvpqo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhoulong.xyz/gtejfhitnm.html

[R11] case 多分支
来源：http://hz.zycfv.cn/gtjiqiiaer.html

case "$1" in
来源：http://hz.wangdashe.top/gtebcsksuj.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtfyqetvdg.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtwcpfwmsh.html

*)     echo "未知命令" ;;
来源：http://hz.9152youxi.cn/gtgtacmmbe.html

esac
来源：http://hz.cqqwz.cn/gtgewyykol.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtssfdbbrn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hywenlv.cn/gthhqrspoe.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtgumlfncx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtiumboosb.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gthtnjyrxd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtqdminidg.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gterflhxuy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtmvvgqqla.html

[R16] until 等待条件
来源：http://hz.meibo888.top/gtdjseghyb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xziqi.cn/gtfowtqqww.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gtpkbrmxcx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xuetiantiany.cn/gtubakpivf.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtwanpslrq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtfvdgcctk.html

[R19] 数组长度
来源：http://hz.ivvv.top/gtcgwirtey.html

echo "${#arr[@]}"
来源：http://hz.sweek.top/gtdrtnwlep.html

[R20] 关联数组（字典）
来源：http://hz.sxryk.cn/gttpzuruqu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigufen.top/gtrdqchgmr.html

[R21] 字符串长度
来源：http://hz.daxiang520.top/gtxeuljqem.html

echo "${#s}"
来源：http://hz.feifeiyinyue.top/gthnyekygh.html

[R22] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtqybggbpn.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gttszaeffx.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtibwosezs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xinyue.icu/gtvltjwqjz.html

[R24] 大小写转换
来源：http://hz.pengpengdd.cyou/gtfibdmpyl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.iojbl.cn/gtmlzcphvv.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtbrmtlrkh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtvxruiqnj.html

[R26] 命令替换
来源：http://hz.hongshengwenyu.top/gtnibnirph.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgfzy.top/gtjejjlufc.html

[R27] 算术展开
来源：http://hz.jianghu66.top/gttyoiwvxl.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtnpwfsuft.html

[R28] 浮点运算
来源：http://hz.xziqi.cn/gtlgdfckov.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtzfckkbma.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtdatazdie.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtgyesfryq.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtzqstwaiy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtgrvuwuis.html

[R31] 局部变量
来源：http://hz.chenjidiqi.icu/gtjkarrxzp.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtugvevmhn.html

[R32] 参数个数校验
来源：http://hz.cucudq.cn/gthmmdscpv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daxiang520.top/gtfaysdlkb.html

[R33] 捕获错误并提示行号
来源：http://hz.hammf.cn/gtjmrnqukh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnqzz.top/gtudraljlg.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtzwtwkzev.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtcrjihqqw.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtsibzttgx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.dianchejie.cn/gtpbsrymlg.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtveqgspgo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtjmzvphma.html

[R37] 把输出赋给变量
来源：http://hz.cucudq.cn/gtnrgawvrd.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtccywfukd.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtuvtmcjcn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zycfv.cn/gtnqzlwgvb.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtrbrbkxrr.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtvyotkaqw.html

[R40] 追加写日志
来源：http://hz.zhoulong.xyz/gtfromatmn.html

echo "log" >> out.log
来源：http://hz.fengsongda.top/gtvyiefavs.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtstmaoyom.html

cmd >/dev/null 2>&1
来源：http://hz.wangdashe.top/gtdjevbfaq.html

[R42] 输入重定向
来源：http://hz.dianchejie.cn/gtihlzcsgz.html

wc -l < a.txt
来源：http://hz.xziqi.cn/gtyhrszezr.html

[R43] 按名字查找文件
来源：http://hz.shzxlz.cn/gtsyhtxhuw.html

find . -name "*.log" -type f
来源：http://hz.svipenyu.cn/gtfbqewnmp.html

[R44] 按修改时间查找
来源：http://hz.zycfv.cn/gtsjnqzohn.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtqvcrfknk.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtsedlaewm.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtvvoewqmv.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtnpynskyt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gtxahalqlj.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtffqtuzgr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gtpvlkfptu.html

[R48] awk 取指定列
来源：http://hz.yangfankeji.com/gtfrmqhqds.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuxming.cn/gtllqyiczn.html

[R49] awk 带条件
来源：http://hz.zdqjudy.top/gtszodoxvx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258.top/gtxalicacl.html

[R50] awk 求和
来源：http://hz.pycfn.com/gthjkxalzj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pycfn.com/gtbvjrxkwb.html

[R51] 排序去重取前几
来源：http://hz.kuanghao11.cn/gteawpsemy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dianchejie.cn/gtqseowxpe.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtxszlocay.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gtsyxxjoru.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gtngrioyps.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.quarkkingdee.top/gteeqqudlv.html

[R54] 比较两个文件
来源：http://hz.yuxming.cn/gtzzoywetp.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gtaufhowdw.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gthcjmloiy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtdhuoemth.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtakddywlh.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtggxjboxe.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtusocbthl.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtwbmsuehj.html

[R58] 下载文件
来源：http://hz.gzhubu.top/gteuobeouf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtaruxezii.html

[R59] 发 POST JSON
来源：http://hz.hnxiangtu.top/gttswqjhre.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gtiobmapvu.html

[R60] 只看 HTTP 状态码
来源：http://hz.meibo888.top/gtegtviscv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtnzmizuku.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtdyaswfni.html


<!-- 参考信息 -->