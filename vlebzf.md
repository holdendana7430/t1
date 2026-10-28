代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.nanxuanxn.top/gtiliwfogj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtkrgztwjn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydzc1.top/gtaoyrxzlh.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gtqqucxgtd.html

SELECT * FROM users;
来源：http://hz.nwbrower.top/gtzjugwpcl.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtxluerxot.html

SELECT id, name FROM users;
来源：http://hz.dianchejie.cn/gtgbbdtirm.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gttkbudwlv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xinyue.icu/gtljjahpaw.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtujgvawrc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jiagoushi.top/gtpvspiomw.html

[Q19] 范围查询
来源：http://hz.fzhhl.top/gttqyyovrz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gtgdbjxroq.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gtnxkyvnar.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtspzvytes.html

[Q21] 空值判断
来源：http://hz.tian-w.cn/gtxgdojgxw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtyxnqpwnc.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gturoiqpjn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtfzjwhepi.html

[Q23] 分页
来源：http://hz.haohaochexian.top/gttjsullux.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigfzy.top/gtvevhscan.html

[Q24] 去重
来源：http://hz.jiagoushi.top/gtpqexagak.html

SELECT DISTINCT city FROM users;
来源：http://hz.xylfe.cn/gtwayioueh.html

[Q25] 只取前 N 条
来源：http://hz.ywan-chungtsiang.top/gtxwaqigwo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zycfv.cn/gtncoturjg.html

[Q26] 计数
来源：http://hz.gotoacloud.top/gtqfzndyxe.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtyevzcqkj.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtkqlkaxkh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxuanxn.top/gtprxlqnsk.html

[Q28] 求和与平均
来源：http://hz.zhoulong.xyz/gtuupgalxg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhongyouzk.top/gtqvynkydt.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtpfjczuka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtkbzbseca.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gtxiqlertt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtlmsarzkv.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtmpidvwqq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuanzhike.top/gtzeuzwodj.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gtfqctvysw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtvpcooxvv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gaohongyu789.top/gtusqkltte.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gtilsucioe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtifigzauj.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtginmatmt.html

SELECT * FROM (
来源：http://hz.daxiang520.top/gtjueqyeqv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.haohaochexian.top/gtoodzuhol.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtzbmmyqff.html

[Q35] 内连接
来源：http://hz.svipenyu.cn/gtiiicpnxa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtlyircimg.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtygnafsxj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.havefunace.top/gtqnnicsaq.html

[Q37] 右连接
来源：http://hz.cashguo.top/gteljcrrem.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtjrvxobwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jlsjyb.cn/gtqxutpciw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.birdmap.top/gtejkaufoc.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigufen.top/gtmyftpepx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.vqdsnc.cn/gtcsgniwla.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sweek.top/gtxevvbosy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtfwkupunt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zycfv.cn/gtunzgpdxl.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtejzjisxp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgfzy.top/gtjqtswghm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtdpsodpqp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.pengpengdd.cyou/gtdzdswjwo.html

[Q42] 连接条件附加过滤
来源：http://hz.daria6918.cn/gtqswmxlnq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.9152youxi.cn/gthlhizqep.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtprwlqkzw.html

[Q43] 标量子查询
来源：http://hz.shanyushiyangtech.top/gtphaitpwi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhoulong.xyz/gtdquyzaoj.html

[Q44] IN 子查询
来源：http://hz.jyoumei.cn/gtsvavpymx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtnkbrfbwx.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gttqmbmfda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtqwouzrbc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtmxpuncyt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtlyrmgzxv.html

[Q47] 与平均值比较
来源：http://hz.ivvv.top/gtybuweqik.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtqcluhbkv.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigufen.top/gtlkrjiobj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xuetiantiany.cn/gtfnhhkzwy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hammf.cn/gtvchhoozt.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtjystidro.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtmtipqkdp.html

[Q50] 批量更新
来源：http://hz.hammf.cn/gtfeognckd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ivvv.top/gthufusney.html

[Q51] 用子查询更新
来源：http://hz.jyoumei.cn/gtwvdzygov.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtjmfkipxw.html

[Q52] 删除指定行
来源：http://hz.0kj1m.cn/gtwwqhpdmw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yangfankeji.com/gtmiixbhhp.html

[Q53] 按条件删除
来源：http://hz.mhx1999.top/gtzntaaaog.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtissnrjiq.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtcsjwqswp.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtjyptawyc.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gttcfawsmg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtpxgwescu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tianlin.xyz/gtxvrvllat.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangtech.top/gtpaayiwlv.html

[Q57] 行号
来源：http://hz.jinqigufen.top/gtifawpnrg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtndojokzz.html

[Q58] 累计求和
来源：http://hz.yongpay.top/gtwasoxprj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxuanxn.top/gtuztvtgar.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtswpkcveo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gogol.net.cn/gthewqviic.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhengqikj.top/gtkptvvrmh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtcisevclo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtekxnhdmv.html

[Q61] 移动平均
来源：http://hz.ydzc1.top/gthquqstfe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hfpthk.cn/gttmgqnrjd.html

[Q62] 分组占比
来源：http://hz.sxryk.cn/gtomgndjwr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtliesfpvj.html

[Q63] 开启事务
来源：http://hz.sufxvd.cn/gteqfvuizv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gttvrnocry.html

[Q64] 提交事务
来源：http://hz.mhx1999.top/gtnewprchb.html

COMMIT;
来源：http://hz.jianghu66.top/gtwcfcxxlf.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtvydtqihg.html

ROLLBACK;
来源：http://hz.xziqi.cn/gtntxtszqp.html

[Q66] 行锁查询
来源：http://hz.yonumen.top/gtrnhfuxmz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtbcxdhnkg.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtdqtfzdlf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.redwolf501.top/gtvozvusen.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtrghadzta.html

SAVEPOINT sp1;
来源：http://hz.yueranfly.top/gthfzbtqfh.html

ROLLBACK TO sp1;
来源：http://hz.mhx1999.top/gtepzbkqly.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtitkkponl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aibaodan.cn/gtwxtuuwkk.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gtfxoslijf.html

ANALYZE TABLE users;
来源：http://hz.jqgufenzy.top/gtjsaahhhu.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtswvrllju.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtisoznvym.html

[Q72] 查看索引
来源：http://hz.zhixingplan.top/gttkixpcsg.html

SHOW INDEX FROM users;
来源：http://hz.xuanzx.com/gtbspekuoh.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtrsgdxzzh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtaotuqwon.html

[Q74] 强制使用索引
来源：http://hz.xuetiantiany.cn/gttyqkdeld.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sweek.top/gtklinpdba.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtcjlielaj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258.top/gtjqgksucb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtwttiemmw.html

[Q76] 按天统计
来源：http://hz.jinghuilouyu.cn/gtkzvleatr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtpmapnsin.html

[Q77] 时间加减
来源：http://hz.bjfxy.top/gtrkpkuxoi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gtlmypiatj.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtejnvudhr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guowangkeji.top/gtklbgebeb.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gtithvzxtl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yangfankeji.com/gtnxcbsvjc.html

[Q80] 字符串截取
来源：http://hz.zhixingplan.top/gtialmnycp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.snrcjt.cn/gtpxalmbls.html

[Q81] 字符串替换
来源：http://hz.guannengcc.top/gtybdwxesy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtwibfeuyi.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtlqbgrkhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtkethgsak.html

[Q83] 大小写转换
来源：http://hz.tian-w.cn/gtgoivucve.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtoozfdawn.html

[Q84] 去除首尾空格
来源：http://hz.shangyingyoupin.top/gtxhgyewxo.html

SELECT TRIM(name) FROM users;
来源：http://hz.aibaodan.cn/gtsocljdon.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtcqcxotmc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gterwmxfvh.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtxefabsgo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yangfankeji.com/gtkubqdfob.html

[Q87] JSON 字段做条件
来源：http://hz.wangshuangyany.cn/gtklmoyrvq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gogol.net.cn/gtzdmbgcdu.html

[Q88] 行转列（条件聚合）
来源：http://hz.meibo888.top/gtoothaltl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtqjmwqxqv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydjk.org.cn/gtyjnxxnmb.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtoztjfijo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtdscanppo.html

[Q90] 生成序号列
来源：http://hz.haohaochexian.top/gtbsgmjjdb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtqqjgxygs.html

================================================================================
来源：http://hz.birdmap.top/gtmowtwliw.html

R. Bash 专题
来源：http://hz.shanyushiyangkeji.top/gtpwyqcqwg.html

================================================================================
来源：http://hz.yongpay.top/gtiokyhdqi.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtqwtncsmb.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtdrszvubh.html

set -euo pipefail
来源：http://hz.wangdashe.top/gtszstvsyk.html

[R02] 变量赋值与使用
来源：http://hz.jyoumei.cn/gtebhdcjjv.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtjghmetyg.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gtbiuknztw.html

readonly PI=3.14
来源：http://hz.sxryk.cn/gtbysckylv.html

[R04] 位置参数
来源：http://hz.quarkkingdee.top/gtsbtwqeyr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtbbzxusux.html

[R05] 参数默认值
来源：http://hz.jinghuilouyu.cn/gtshgcynbr.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtxcxfsdkq.html

[R06] 判断命令是否存在
来源：http://hz.zhengqikj.top/gtdgbcbazn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtuvbythzn.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtdldkzgbr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.feifeiyinyue.top/gtpselfohq.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtmmbngqtj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtumnblgkz.html

[R09] 字符串比较
来源：http://hz.chenzaomai.com/gtqbeeabso.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenjidiqi.icu/gtfnhzgbwv.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtbgubzbcz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtxzbaqdqo.html

[R11] case 多分支
来源：http://hz.tanke756.top/gtktcccngf.html

case "$1" in
来源：http://hz.chenzaomai.com/gtcbdvkfrh.html

start) echo "启动" ;;
来源：http://hz.nanxinkj.top/gtqgtmufib.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtirdbvath.html

*)     echo "未知命令" ;;
来源：http://hz.sysykeji.top/gtlkvrywhn.html

esac
来源：http://hz.snrcjt.cn/gtmydrvpfe.html

[R12] for 遍历文件
来源：http://hz.andypj.xyz/gtztrivfdy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ybcxt.top/gttvusnqwd.html

[R13] for 计数循环
来源：http://hz.snrcjt.cn/gtoprlxcuh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtkosgstve.html

[R14] C 风格 for
来源：http://hz.zhoulong.xyz/gtijoswpqz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtyxbgnhla.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gtqdtrbimq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtuhvjzfdk.html

[R16] until 等待条件
来源：http://hz.shzxlz.cn/gtzvlabgzc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtcbinkvni.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtlrjfebfr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.52xcode.cn/gtlogsjhsd.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtjnfottkt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sxryk.cn/gtjayfxmnb.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtdvjxcoqb.html

echo "${#arr[@]}"
来源：http://hz.zhoulong.xyz/gtifbrkzsm.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtyzhifzzk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhijiandao.cn/gtjngkowdd.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtdbyqjhdc.html

echo "${#s}"
来源：http://hz.chenjidiqi.icu/gtkpvmkbpp.html

[R22] 截取子串
来源：http://hz.jlsjyb.cn/gtgnabnddv.html

echo "${s:0:5}"
来源：http://hz.fzhhl.top/gtcruwkwqz.html

[R23] 字符串替换
来源：http://hz.gzhubu.top/gtjyubvzdt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gttmsxygxr.html

[R24] 大小写转换
来源：http://hz.chenzaomai.com/gtatcvnfyo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daxiang520.top/gtqhccvray.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gtzwcnckii.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhixingplan.top/gtamhjypet.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gtbgcxqiji.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtahgrdyij.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtjbbnxfmu.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtzjrgjxvd.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtjiwogyfd.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtiqrcwkqh.html

[R29] 定义函数
来源：http://hz.gotoacloud.top/gtuigrrahq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.vqdsnc.cn/gtjvtslqmw.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtbxepkvrf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gogol.net.cn/gtiotwtcik.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtsrpdfvor.html

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gtqqswssob.html

[R32] 参数个数校验
来源：http://hz.iojbl.cn/gtswoadsgz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sweek.top/gtlhdlvumk.html

[R33] 捕获错误并提示行号
来源：http://hz.quarkkingdee.top/gtcoqthrob.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtxffejkjz.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtggulklci.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtjcxqopho.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtyudqcqzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtalogzgih.html

[R36] 并发执行多个任务
来源：http://hz.daxiang520.top/gtrinjguhp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtbglsnhbf.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtjglgffuh.html

files=$(ls -1)
来源：http://hz.gzhubu.top/gtawkalwxa.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtwwpxbozq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.kuanghao11.cn/gtcioqldny.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtxhuuybqr.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtfzoesnqj.html

[R40] 追加写日志
来源：http://hz.dianchejie.cn/gtglvxaqvy.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtuevailfp.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtzqzviotq.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtdrdzauqp.html

[R42] 输入重定向
来源：http://hz.daxiang520.top/gtngaaqmpz.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtqqathshx.html

[R43] 按名字查找文件
来源：http://hz.gotoacloud.top/gtfczcmabd.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gtdhdyitwi.html

[R44] 按修改时间查找
来源：http://hz.sysykeji.top/gtuspizemh.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gttsqkhpae.html

[R45] 批量删除
来源：http://hz.jinqigfzy.top/gtgeeseagh.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtqcjhdakr.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtrmjugacr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtazjefiwr.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtmbprrydm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtpxxlbzrg.html

[R48] awk 取指定列
来源：http://hz.zhijiandao.cn/gtmmmxrcto.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtmdiqjwvk.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtztqicjdn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtglfdvbdl.html

[R50] awk 求和
来源：http://hz.nwbrower.top/gtczzsrivk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhiwuduotai.top/gttqaiasfb.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gtspysabke.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cdnleiting.top/gtmffjrdtm.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtqkkylvyq.html

wc -l a.txt
来源：http://hz.bjfxy.top/gtdaflmbuq.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gtgiictbmo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gthbsuploc.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gtuufndhdj.html

diff a.txt b.txt
来源：http://hz.quarkkingdee.top/gtwotkcagz.html

[R55] 压缩与解压
来源：http://hz.tian-w.cn/gtjaixymnx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtasbkmdwi.html

[R56] 远程拷贝
来源：http://hz.cucudq.cn/gthwyuilbx.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtzwujwwdz.html

[R57] 远程执行命令
来源：http://hz.jianghu66.top/gtrnuzdzwo.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gttheybtxl.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtsfmlgxjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gthibrcatg.html

[R59] 发 POST JSON
来源：http://hz.feifeiyinyue.top/gtrehbviyw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hongshengwenyu.top/gtmhsimlzn.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtybntbuli.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gthucrogzt.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtmyvffxfe.html

df -h;  du -sh *
来源：http://hz.tian-w.cn/gtpzkgzrov.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtyvfpxiwy.html

du -ah . | sort -rh | head -10
来源：http://hz.dianchejie.cn/gtulyurrve.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtbfsaxcyg.html


<!-- 参考信息 -->