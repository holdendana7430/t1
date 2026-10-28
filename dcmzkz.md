代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtldfelhdk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.chenlongwang.top/gtyddtoxbo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtilcvknre.html

[Q15] 查询全部
来源：http://hz.c1oappe.top/gteqnuycky.html

SELECT * FROM users;
来源：http://hz.zhixingplan.top/gtqxmnbacq.html

[Q16] 查询指定列
来源：http://hz.zhijiandao.cn/gtrcevntou.html

SELECT id, name FROM users;
来源：http://hz.zdqjudy.top/gtgtjrdxmn.html

[Q17] 条件查询
来源：http://hz.daxiang520.top/gtzdnyzuht.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gttvgiafnp.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtdvmynwkj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhongyouzk.top/gtzbwjorgc.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gtstaskooq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daria6918.cn/gtdfelntue.html

[Q20] IN 列表
来源：http://hz.0kj1m.cn/gtjdesfgqb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jlsjyb.cn/gtxasiawgq.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtstmwuebb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ydjk.org.cn/gtitmftodg.html

[Q22] 排序
来源：http://hz.yuxming.cn/gtkzzmyiqj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtipultlwm.html

[Q23] 分页
来源：http://hz.daria6918.cn/gtsdzmymck.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuanzx.com/gtmrrrnuxq.html

[Q24] 去重
来源：http://hz.quarkkingdee.top/gtdewgialx.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtspnaffab.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gtjtrefcuc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xingfuxueyuan.xyz/gtmycpsidh.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtohnqmkpf.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnxiangtu.top/gtodnlxetw.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtvdhripfw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shangyingyoupin.top/gtgiugkgzk.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtrpukhytk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.pengpengdd.cyou/gtyijtlrpm.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gttpkwubzz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtiirlzztt.html

[Q30] 分组统计
来源：http://hz.birdmap.top/gtmcwkbjpv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gttjerzjwx.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gtaruhsxjp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jqgfzy.top/gtyrxhdmxm.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtcdnahzhc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtcmguchgx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtnnwnhoti.html

[Q33] 多列分组
来源：http://hz.cheryme.top/gtfqdebpdy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtkhaoerlc.html

[Q34] 每组取第一条
来源：http://hz.yj20258888.top/gtfdwzimvt.html

SELECT * FROM (
来源：http://hz.ppjwa.cn/gtxrwigjhy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jyoumei.cn/gtnauewkws.html

) t WHERE rn = 1;
来源：http://hz.c1oappe.top/gtlprnzzxs.html

[Q35] 内连接
来源：http://hz.yonumen.top/gtzreyorzt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtrsgdpxpf.html

[Q36] 左连接
来源：http://hz.yanxiufei.cn/gtrqharggb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtvuqupksp.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtclhxfejh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinqigufen.top/gtcilqkkam.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yvedp.cn/gtbztkinpx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtedxrzxyx.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gthpradwkl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.316326.xyz/gtwhjhmfwl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinghuilouyu.cn/gtluyeektu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gtinoccbmq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenlongwang.top/gthotegzdk.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtaxcpcwba.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.iojbl.cn/gtjoxiccav.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuanzx.com/gthxbzpbyh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtkpvtvqxc.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxinkj.top/gtoumukryb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenjidiqi.icu/gtndzdvver.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtjqbkxajl.html

[Q43] 标量子查询
来源：http://hz.wangshuangyany.cn/gtgvnydqcq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258888.top/gtdifmwhul.html

[Q44] IN 子查询
来源：http://hz.zdqjudy.top/gtjaxqmwkp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tanke756.top/gtzlvvsjax.html

[Q45] EXISTS 判断存在
来源：http://hz.yonumen.top/gtcxdpulid.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtixmzqmow.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhiwuduotai.top/gtbfxgxotl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtscvxqyun.html

[Q47] 与平均值比较
来源：http://hz.yangfankeji.com/gtowmrvzue.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cqqwz.cn/gtkroynlfs.html

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gtynlyisml.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sweek.top/gtqhsldtck.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtrhbplnln.html

[Q49] 更新单行
来源：http://hz.vqdsnc.cn/gtyrctcben.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtxbubkbql.html

[Q50] 批量更新
来源：http://hz.bjfxy.top/gtfgysrvra.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.snrcjt.cn/gtgiqyqinh.html

[Q51] 用子查询更新
来源：http://hz.jqgfzy.top/gtenplkamr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtngqeglug.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gtealhcoir.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jianghu66.top/gtqnvrsewu.html

[Q53] 按条件删除
来源：http://hz.zhixingplan.top/gtmbjlqrvl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtrevozncv.html

[Q54] 清空表
来源：http://hz.jinghuilouyu.cn/gtjoljjnxu.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtiovmtzbu.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtcfpjedjr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangtech.top/gtvvtkoqxi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sxryk.cn/gtkmnsuhhs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtxqeznajj.html

[Q57] 行号
来源：http://hz.hnqzz.top/gtglcuvxkf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtankidqzv.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gtsilroxhn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shangyingyoupin.top/gtmgxwzpoh.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gthlbsxmwp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xinyue.icu/gtifeyerjn.html

[Q60] 取上一行 / 下一行
来源：http://hz.shuidangran.top/gtsvexvjfs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yuxming.cn/gtibcttruq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnxiangtu.top/gthkihrist.html

[Q61] 移动平均
来源：http://hz.aizwys.cn/gthcqtsdda.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pengpengdd.cyou/gtdmmfehjz.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtuhsxhnhw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtzyrcyywq.html

[Q63] 开启事务
来源：http://hz.tianlin.xyz/gtrwtvlseo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtakpbcutt.html

[Q64] 提交事务
来源：http://hz.jqgufenzy.top/gtxenbcqsk.html

COMMIT;
来源：http://hz.xylfe.cn/gtdmuypscv.html

[Q65] 回滚事务
来源：http://hz.cheryme.top/gteghiadbr.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtgoxmjfgi.html

[Q66] 行锁查询
来源：http://hz.aibaodan.cn/gtfznxdkfv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jqgufenzy.top/gtkupiylmx.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtvfvhtikt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtyuhzoybe.html

[Q68] 保存点
来源：http://hz.pycfn.com/gtdbvtroah.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtjxsxwdlq.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtsdzzjynw.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gtnfmslonu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ehwqpu.com/gthzkfzalq.html

[Q70] 更新统计信息
来源：http://hz.haohaochexian.top/gttdzscqnp.html

ANALYZE TABLE users;
来源：http://hz.svipenyu.cn/gtgyoubblm.html

[Q71] 查看建表语句
来源：http://hz.birdmap.top/gtbwshuzvq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtcpmpceol.html

[Q72] 查看索引
来源：http://hz.dashuyun.cn/gtiabocumt.html

SHOW INDEX FROM users;
来源：http://hz.aizwys.cn/gtykekulhr.html

[Q73] 查看表状态
来源：http://hz.gogol.net.cn/gtvajlmowi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtwkeuvlcf.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtfdvomvdg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtykwlguqu.html

[Q75] 日期格式化
来源：http://hz.yueranfly.top/gttuhanpfu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tanke756.top/gtpwcbmgzu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.feifeiyinyue.top/gtezevshjv.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtbxngeltw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gttombgxfp.html

[Q77] 时间加减
来源：http://hz.jqgfzy.top/gtudanurif.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gzhubu.top/gtwqgmdqpt.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtejxuwwbx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtndpycdeh.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtwfctpdgb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gttbdphbdf.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtwkwehzbu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258.top/gtxrhzqtrd.html

[Q81] 字符串替换
来源：http://hz.svipenyu.cn/gtezlvgolj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jianghu66.top/gtcbworarj.html

[Q82] 字符长度与字节长度
来源：http://hz.gzhubu.top/gtbnmysxlu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gtrcuvbdhn.html

[Q83] 大小写转换
来源：http://hz.feifeiyinyue.top/gtoniapibm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtxexijrvw.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtbmyddmmb.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtvczkpgod.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtggfholuy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtezylrbhu.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtcvelftou.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.iojbl.cn/gtrslxqtsv.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtwdlhgfkr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtujtrufxl.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtgmrzpunc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gtnxikipjt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gtqlalaglj.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gttrwlukjl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtamcwawpp.html

[Q90] 生成序号列
来源：http://hz.yuanzhike.top/gtyhevaxui.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cheryme.top/gtmsquaruh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkvmxlfdw.html

R. Bash 专题
来源：http://hz.tanke756.top/gtanjssdtu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgzqsanmb.html

[R01] shebang 与严格模式
来源：http://hz.mhx1999.top/gtaisuuorz.html

#!/usr/bin/env bash
来源：http://hz.zhixingplan.top/gtqfwunupe.html

set -euo pipefail
来源：http://hz.xziqi.cn/gtppaqttyd.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gtsfllrfni.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtvlmjqkvh.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gtbptvlrwh.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gtvhvgiiyv.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtdbrceyye.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtndhkqkmt.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtdemoywkp.html

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gthrzgoxxs.html

[R06] 判断命令是否存在
来源：http://hz.haohaochexian.top/gtfayrvyyf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtcjnwhjks.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtafenbpnk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cqqwz.cn/gtviyuouln.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtcjsgyllm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtztstseeu.html

[R09] 字符串比较
来源：http://hz.zhiwuduotai.top/gtvxopqwwv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.wangdashe.top/gtbgvfsxlm.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gtbovmnlpi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnxiangtu.top/gteaeyynhe.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtmgzjtvpg.html

case "$1" in
来源：http://hz.fengsongda.top/gtdjgwdvvx.html

start) echo "启动" ;;
来源：http://hz.dianchejie.cn/gtbiuzoqbi.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtdpwdemlt.html

*)     echo "未知命令" ;;
来源：http://hz.birdmap.top/gtkwjjavml.html

esac
来源：http://hz.fengsongda.top/gtjqlkgpxn.html

[R12] for 遍历文件
来源：http://hz.tanke756.top/gtzyyfjmrm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shuidangran.top/gtedyqfvwj.html

[R13] for 计数循环
来源：http://hz.birdmap.top/gtslxgqexh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gtubybhuvl.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gtybdctysn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtiucdraan.html

[R15] while 逐行读文件
来源：http://hz.zhoulong.xyz/gtkqhqhebt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtdlccyiir.html

[R16] until 等待条件
来源：http://hz.pycfn.com/gtvjxqryfe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gtftrdxzoy.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtrbhetsqt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tian-w.cn/gttkyfjiuw.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtfejhieaj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtbfipyjoq.html

[R19] 数组长度
来源：http://hz.gogol.net.cn/gtfdbfnhkt.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gtkkgpmzbn.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtwcfjnnyy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtmbtxosee.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtrchrrqha.html

echo "${#s}"
来源：http://hz.zhiwuduotai.top/gtudrylses.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtnshhczhr.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtxfjbstvb.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtikchtegx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtlhkydgdw.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtrcazymub.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gtefiijpbc.html

[R25] 去后缀 / 去前缀
来源：http://hz.sxryk.cn/gtgbwtaykq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pycfn.com/gtkzwxgwau.html

[R26] 命令替换
来源：http://hz.zhixingplan.top/gtovmompxf.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtkhreldod.html

[R27] 算术展开
来源：http://hz.hnqzz.top/gtefdupnbg.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtruuwqygj.html

[R28] 浮点运算
来源：http://hz.shuidangran.top/gtyurcqojv.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtcdybupzy.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtrpsxdgdv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258.top/gtqizudkyc.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gtesklymgz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydjk.org.cn/gtlrtlzywa.html

[R31] 局部变量
来源：http://hz.gogol.net.cn/gtltmzdhhu.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtgiemsoiy.html

[R32] 参数个数校验
来源：http://hz.yuanzhike.top/gtcermllky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtruzztofl.html

[R33] 捕获错误并提示行号
来源：http://hz.yangfankeji.com/gtrgqfbvdp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtoehhkgfy.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtembebycs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtkzdzvvie.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtzqjzydsr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhaomingkeji.xyz/gtecgscttp.html

[R36] 并发执行多个任务
来源：http://hz.hnqzz.top/gtilvzyzcn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtfxqtlhoh.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gtzplfetdd.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtmtnolebq.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtmjxajwfp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtmnqroxah.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtnabtjwyk.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtgtefprbs.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtasdkfohm.html

echo "log" >> out.log
来源：http://hz.ehwqpu.com/gtzpajumwz.html

[R41] 丢弃输出
来源：http://hz.feifeiyinyue.top/gtlglpxdsb.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtorvjewek.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtykhncloe.html

wc -l < a.txt
来源：http://hz.yvedp.cn/gtrldbvxhd.html

[R43] 按名字查找文件
来源：http://hz.zdqjudy.top/gtffsxnlwv.html

find . -name "*.log" -type f
来源：http://hz.nanxuanxn.top/gtfobdcibj.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtnwzhigok.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gterdrjqbe.html

[R45] 批量删除
来源：http://hz.316326.xyz/gtlhpyefcu.html

find . -name "*.tmp" -delete
来源：http://hz.andypj.xyz/gtqbevcnoq.html

[R46] 递归替换文件内容
来源：http://hz.feifeiyinyue.top/gttvjlgwgq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gthhognhrm.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gthsaxupjf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.kuanghao11.cn/gtschhgwfe.html

[R48] awk 取指定列
来源：http://hz.sxryk.cn/gtjxwvoccu.html

awk '{print $1, $3}' a.txt
来源：http://hz.chenjidiqi.icu/gtrwekrpjx.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtqmunvkxj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtrhycsifo.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtkgoqvngp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtxubgubnz.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtzhggafxc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yueranfly.top/gtkpfiihqc.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtakzvyzet.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtaimuxtpd.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtxwjhhxfw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnxiangtu.top/gtfsmnhunc.html

[R54] 比较两个文件
来源：http://hz.guannengcc.top/gthbkztgby.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtyikyyvgq.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtowykxiuo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtqxxscoqd.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtzlpugdhe.html

scp file user@host:/path/
来源：http://hz.dianchejie.cn/gtnavljldv.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtaffdysod.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gtkitwrvwz.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtfbxdbvao.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tianlin.xyz/gtcdiglqja.html

[R59] 发 POST JSON
来源：http://hz.iojbl.cn/gtbrfdmvrt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnxiangtu.top/gtqokywclg.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gthyhivnpv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtcwqsmmwh.html

[R61] 磁盘占用
来源：http://hz.fengsongda.top/gtfqzuthui.html

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gtrjznouuv.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtmfbywspf.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtqdmbcbna.html

[R63] 内存与进程
来源：http://hz.birdmap.top/gtnulvymsd.html


<!-- 参考信息 -->