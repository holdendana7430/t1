代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.xuetiantiany.cn/gtdlyuiujn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.kuanghao11.cn/gtinjhtuse.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tian-w.cn/gtmuyeulwq.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtlojuiwta.html

SELECT * FROM users;
来源：http://hz.guannengcc.top/gtsbwneoqh.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtjxszfwgi.html

SELECT id, name FROM users;
来源：http://hz.ybcxt.top/gtztpbjdaq.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtirxmsqin.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtexnynuch.html

[Q18] 模糊匹配
来源：http://hz.hywenlv.cn/gtspnuqzqf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gtvbuqgqzb.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtmhlsiyhw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gtxaqzobls.html

[Q20] IN 列表
来源：http://hz.gotoacloud.top/gtxfqtpwue.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gtjbhssjqc.html

[Q21] 空值判断
来源：http://hz.gaohongyu789.top/gtqeabdilz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.9152youxi.cn/gteqalujwq.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gtqchhwrcg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gttagtxmwh.html

[Q23] 分页
来源：http://hz.cheryme.top/gtxclmxeab.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgufenzy.top/gtnrukvykn.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gtpsuxdlmq.html

SELECT DISTINCT city FROM users;
来源：http://hz.cdnleiting.top/gtinsbyhqf.html

[Q25] 只取前 N 条
来源：http://hz.fengsongda.top/gtegrvndgd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pengpengdd.cyou/gtoouqavvu.html

[Q26] 计数
来源：http://hz.yangfankeji.com/gtffukvekl.html

SELECT COUNT(*) FROM users;
来源：http://hz.chenlongwang.top/gtbrtfqash.html

[Q27] 条件计数
来源：http://hz.jiagoushi.top/gtqhpvgsmb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jiagoushi.top/gtkchlwojf.html

[Q28] 求和与平均
来源：http://hz.zhongyouzk.top/gtfmleekzf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtladwdgyt.html

[Q29] 最大最小值
来源：http://hz.wangshuangyany.cn/gtnuuiuawu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtvitzwghm.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtdwkijrdd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtdavwyjzc.html

[Q31] 分组后过滤
来源：http://hz.yangfankeji.com/gthhnuyfpb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gtjmfuzyvu.html

[Q32] 分组拼接字符串
来源：http://hz.0kj1m.cn/gtyegajgit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtswvuhfyg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtgarkajux.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtfclljvzc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.snrcjt.cn/gtjafjhfsy.html

[Q34] 每组取第一条
来源：http://hz.nanxinkj.top/gtbyniopxz.html

SELECT * FROM (
来源：http://hz.ehwqpu.com/gtrilgnzbw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gzhubu.top/gtpuhwnggv.html

) t WHERE rn = 1;
来源：http://hz.hywenlv.cn/gtilspzrsc.html

[Q35] 内连接
来源：http://hz.zdqjudy.top/gtxldcbfeo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtanhteorz.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtsuvzgxqt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtshjhcvum.html

[Q37] 右连接
来源：http://hz.yongpay.top/gteoznaypr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtgytggcnk.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zdqjudy.top/gtyawoospn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cashguo.top/gtzgzeqbaa.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtsawkrmal.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ywan-chungtsiang.top/gtjkguqjyj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtcilyzlne.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtdmlecgpd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtkgmselqv.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtviigvwsm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gzhubu.top/gtpryaybii.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtytpffass.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xziqi.cn/gtcuibbqov.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gtdbkjcjqg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258.top/gtgehflupd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhiwuduotai.top/gtembangcj.html

[Q43] 标量子查询
来源：http://hz.kuanghao11.cn/gtbysgkmcp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gtkyxtmgyt.html

[Q44] IN 子查询
来源：http://hz.xuetiantiany.cn/gtvjpcrzke.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gtnuknjqyz.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtbwolatrx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gthrflfqij.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtavamxmyl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sysykeji.top/gtcrpvvghc.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtrbfunctw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtljjuwcxg.html

[Q48] CTE 公用表表达式
来源：http://hz.xziqi.cn/gtrklqipqe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gotoacloud.top/gtbldslozu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtafngxeth.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtaaoufazi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ivvv.top/gtfzmghmko.html

[Q50] 批量更新
来源：http://hz.52xcode.cn/gtkqgoqqxu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtblexnmpo.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gtyfjehgzy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.vqdsnc.cn/gtxhxpbhla.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtikwwzbct.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guannengcc.top/gtfaavoweu.html

[Q53] 按条件删除
来源：http://hz.zhijiandao.cn/gtyupqhnrq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fengsongda.top/gtjmcelinb.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gtdvgualre.html

TRUNCATE TABLE logs;
来源：http://hz.sufxvd.cn/gtuqlrpywk.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtwuwfowfc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.dashuyun.cn/gtzoqztlab.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenzaomai.com/gttlqbqxll.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangshuangyany.cn/gtonnozdbu.html

[Q57] 行号
来源：http://hz.gotoacloud.top/gtzwediroe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtksbminxk.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtsamfaqvd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yj20258.top/gtkxvcmfqv.html

[Q59] 分组内累计
来源：http://hz.ivvv.top/gtvalowbwr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtjoizezgr.html

[Q60] 取上一行 / 下一行
来源：http://hz.jqgfzy.top/gthxkffqdy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nanxuanxn.top/gtqogscofd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtnwbuhrjr.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtkjfvhffo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtunnhipmc.html

[Q62] 分组占比
来源：http://hz.jinghuilouyu.cn/gtmfeskpbk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shuidangran.top/gtqutilmoy.html

[Q63] 开启事务
来源：http://hz.yueranfly.top/gtrgyplrlt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.316326.xyz/gtgdhimhdj.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gteyslqxlp.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtrfuqujbs.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtvwoszepc.html

ROLLBACK;
来源：http://hz.shangyingyoupin.top/gtdkeqillo.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gthnqomwiz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guannengcc.top/gtaysykkti.html

[Q67] 设置隔离级别
来源：http://hz.tanke756.top/gtpocdadyn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jinyuanbaomall.cn/gtpfsjnrjg.html

[Q68] 保存点
来源：http://hz.52xcode.cn/gtxfwxfzrj.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gthdhwyefi.html

ROLLBACK TO sp1;
来源：http://hz.tian-w.cn/gtjagtwmun.html

[Q69] 查看执行计划
来源：http://hz.dashuyun.cn/gtyulgenqp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gtpllitjkw.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtmimzgnsh.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtlavrcjfd.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtlzpkepxb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtwilkyyrp.html

[Q72] 查看索引
来源：http://hz.zhiwuduotai.top/gtqtuppkxr.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtchutnaxz.html

[Q73] 查看表状态
来源：http://hz.sweek.top/gtdtbleiyr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtokjhkwjg.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gtdxwrtfsi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtufaevnna.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtaupdwbgm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xziqi.cn/gtcnddmxty.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aizwys.cn/gtbcmrfrbm.html

[Q76] 按天统计
来源：http://hz.birdmap.top/gtwjhgelhh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guannengcc.top/gtdwqswzim.html

[Q77] 时间加减
来源：http://hz.zhengqikj.top/gtacyzfkwv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuxming.cn/gtaigzmeis.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtzwpmezgh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.redwolf501.top/gtyygyojkp.html

[Q79] 字符串拼接
来源：http://hz.0kj1m.cn/gtdwkdzbmh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhoulong.xyz/gtontywhol.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtozcfqhng.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtonetukoj.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtzygqpnmw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtenyuwbxf.html

[Q82] 字符长度与字节长度
来源：http://hz.guowangkeji.top/gtwhgeifct.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gthefqpikm.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtrlqywmwa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guowangkeji.top/gtwhbyrifq.html

[Q84] 去除首尾空格
来源：http://hz.ydjk.org.cn/gtxjecbyuz.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtsfxtoqfb.html

[Q85] 数值取整
来源：http://hz.xziqi.cn/gtttgaxfet.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yuxming.cn/gtysqcwfag.html

[Q86] 读取 JSON 字段
来源：http://hz.zycfv.cn/gtmsenzebj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydjk.org.cn/gtvaldmzpq.html

[Q87] JSON 字段做条件
来源：http://hz.sufxvd.cn/gtxbmjmwyu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gzhubu.top/gtkepllltt.html

[Q88] 行转列（条件聚合）
来源：http://hz.c1oappe.top/gtpjjycddq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gtriwforyy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhoulong.xyz/gtkbjallxj.html

[Q89] 判断表是否存在
来源：http://hz.pengpengdd.cyou/gtmkfbuamg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pycfn.com/gtsjcwcxtp.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtvrhiiltx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtvwrtlixz.html

================================================================================
来源：http://hz.jyoumei.cn/gtmaaqdrco.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtddaictst.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwasjtpas.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gtuhjbyesg.html

#!/usr/bin/env bash
来源：http://hz.aizwys.cn/gtqggqzdng.html

set -euo pipefail
来源：http://hz.jlsjyb.cn/gtozwcuzwe.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtsdqwoody.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtdkdcgduh.html

[R03] 只读变量
来源：http://hz.cheryme.top/gtabvpwcyx.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtegcgyroc.html

[R04] 位置参数
来源：http://hz.tanke756.top/gtagdpschc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydzc1.top/gtkwmiqbri.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtnoqetqwn.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gtgyfxpzov.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gttegvexxr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtqowvmhrr.html

[R07] if 判断文件
来源：http://hz.yueranfly.top/gtafcyzikh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtaiqwypra.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtapctxvew.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtpgmdybeo.html

[R09] 字符串比较
来源：http://hz.dashuyun.cn/gtdtoztzix.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtizkgfuon.html

[R10] 正则匹配
来源：http://hz.wangshuangyany.cn/gteqaohymd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtowuayhem.html

[R11] case 多分支
来源：http://hz.yanxiufei.cn/gtlwuchmay.html

case "$1" in
来源：http://hz.mhx1999.top/gtvulthvso.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gtdxyeldrs.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtwdnwlliu.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtkxmtwcmo.html

esac
来源：http://hz.zhijiandao.cn/gtyzthoqcb.html

[R12] for 遍历文件
来源：http://hz.zhixingplan.top/gtlmaierlt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtlhmggedh.html

[R13] for 计数循环
来源：http://hz.52xcode.cn/gttxumtjbw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gthnadntcu.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtzociwgfb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aizwys.cn/gtvysmgtyk.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtjgmlyowy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtzipwpaez.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtoxclzaxq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtwtkvwxky.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtcthfiysp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtfjgzpikz.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gttcrotrpq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gticxeudrz.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtbmxniiqr.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangtech.top/gtufpejhdj.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtwctolacu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtjcximlsz.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtasithcmb.html

echo "${#s}"
来源：http://hz.zhixingplan.top/gtkqyzzudt.html

[R22] 截取子串
来源：http://hz.sxryk.cn/gtxagkwwkz.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtlwpnogca.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtjstdzfao.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtdkenoshe.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtmmhciwit.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtwwlxtfbh.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gtupwbpcsm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gtdxhavcyq.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtxjgqwase.html

now=$(date +%F); echo "$now"
来源：http://hz.gotoacloud.top/gtrrrwfrld.html

[R27] 算术展开
来源：http://hz.jinyuanbaomall.cn/gtvsvjwikf.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtphlxfckh.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtquccacyn.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtoigymnlq.html

[R29] 定义函数
来源：http://hz.ybcxt.top/gtijrpqcga.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtewrolzay.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtmxkzlvij.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fengsongda.top/gtbxmgqqbe.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtdtnrrjao.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxinkj.top/gtrczlmrux.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gtoirxzjfd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hysaishi.cn/gtjsxmzwzo.html

[R33] 捕获错误并提示行号
来源：http://hz.guowangkeji.top/gtpodysoae.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinghuilouyu.cn/gtijbtufyj.html

[R34] 退出时清理
来源：http://hz.guannengcc.top/gtwdhkufnm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtntosmafn.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtpyeshkcc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yvedp.cn/gteosnlwkt.html

[R36] 并发执行多个任务
来源：http://hz.chenlongwang.top/gtojkywkfv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtrytfjckt.html

[R37] 把输出赋给变量
来源：http://hz.haohaochexian.top/gtkhkoszeb.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtgfaqcqek.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtwcxgsnsg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gtmslequzz.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gtkqobcizc.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtjkdfipgi.html

[R40] 追加写日志
来源：http://hz.jyoumei.cn/gtxdbidnip.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtyipzskgv.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtjfrvzxyv.html

cmd >/dev/null 2>&1
来源：http://hz.shuidangran.top/gteyerxqvw.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtjlajimtq.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtzuxfmmoe.html

[R43] 按名字查找文件
来源：http://hz.wangshuangyany.cn/gtndoyizxt.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtcntfccfd.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gtsztglarg.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtbihjctan.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtmvztcinl.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtskmfhjrv.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gtjrymnwea.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtlyetdjyw.html

[R47] sed 单行替换
来源：http://hz.xylfe.cn/gtchtmsdvx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xziqi.cn/gtecmqecpk.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtafjxbfha.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtwketzqyu.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtkznfvkrp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.mhx1999.top/gthwqcofev.html

[R50] awk 求和
来源：http://hz.ydzc1.top/gtplehnvad.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtttdvkyvj.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtaxideldp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuanzx.com/gtekitnrtz.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtzzdcakun.html

wc -l a.txt
来源：http://hz.smart0.xyz/gtnykzghym.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtsfhoewun.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtzijsgmwk.html

[R54] 比较两个文件
来源：http://hz.jyoumei.cn/gtamnjluvr.html

diff a.txt b.txt
来源：http://hz.xylfe.cn/gtwvxsbilh.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtbutzhihc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtpzkaufox.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtqmfpyouy.html

scp file user@host:/path/
来源：http://hz.yvedp.cn/gtryalsgky.html

[R57] 远程执行命令
来源：http://hz.hysaishi.cn/gtmofidcty.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtebkavnvt.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtfxdsnbps.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtjswxnial.html

[R59] 发 POST JSON
来源：http://hz.zycfv.cn/gtwucogwkx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gturgnfqxi.html

[R60] 只看 HTTP 状态码
来源：http://hz.52xcode.cn/gtmaxgccdw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtfbhukpel.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtjrfxabpw.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gtjdbqklqb.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtvgkqgxcp.html

du -ah . | sort -rh | head -10
来源：http://hz.hammf.cn/gtaiwvsinq.html

[R63] 内存与进程
来源：http://hz.svipenyu.cn/gtgndklesd.html


<!-- 参考信息 -->