代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sufxvd.cn/gteilsbric.html

[Q18] 模糊匹配
来源：http://hz.jqgfzy.top/gtvguynlhk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhaomingkeji.xyz/gtiyxqebyo.html

[Q19] 范围查询
来源：http://hz.yvedp.cn/gtxbetvgjb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgufenzy.top/gtlkcgiqgw.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtrzhdupzr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtyhpfsvcp.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtgmblbxtq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gtvqbkpljl.html

[Q22] 排序
来源：http://hz.snrcjt.cn/gthmfwvtls.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxuanxn.top/gtfcbzlxsk.html

[Q23] 分页
来源：http://hz.guannengcc.top/gtkhfykian.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtumfynzqy.html

[Q24] 去重
来源：http://hz.hongshengwenyu.top/gtubeslzkw.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtrofssxci.html

[Q25] 只取前 N 条
来源：http://hz.hnxiangtu.top/gtyckuejap.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.daria6918.cn/gtmwmzidoi.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtjuyfmgst.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtrttuejio.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtftuchazc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.birdmap.top/gtueidwjyw.html

[Q28] 求和与平均
来源：http://hz.svipenyu.cn/gtmnfkymkb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gturveadqw.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtgxapydzd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gtubzzhkje.html

[Q30] 分组统计
来源：http://hz.meibo888.top/gtjlzietve.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gttdgdwwut.html

[Q31] 分组后过滤
来源：http://hz.xylfe.cn/gtnwocwwzo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.birdmap.top/gtyksnrfbk.html

[Q32] 分组拼接字符串
来源：http://hz.yanxiufei.cn/gtlgvjkteb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtpgczcdax.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sxryk.cn/gtwxjqxemm.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtamxvafec.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtmrwuxavh.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtcnhoelxi.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gtdwreabqg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cdnleiting.top/gtoycjzoxq.html

) t WHERE rn = 1;
来源：http://hz.svipenyu.cn/gtnxrdjrzn.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtoaezeebo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtsbhyxcif.html

[Q36] 左连接
来源：http://hz.mhx1999.top/gtlpammoyn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gthunjlxbh.html

[Q37] 右连接
来源：http://hz.yuxming.cn/gtttwnrytu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shuidangran.top/gtikcutosv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtxtypvqdt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hysaishi.cn/gtqlgtvrmc.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtraqagmyk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gtveboudng.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.dashuyun.cn/gttgjunuvc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtuamafgly.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cheryme.top/gttjcqpzzs.html

[Q41] 多表连接
来源：http://hz.nanxuanxn.top/gtxnehujhj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtfoplylxv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.aibaodan.cn/gtizfxapql.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xinyue.icu/gtnplunses.html

[Q42] 连接条件附加过滤
来源：http://hz.xinyue.icu/gtoxqgmuzi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gzhubu.top/gtcmgoltaa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yanxiufei.cn/gtuxqiwggv.html

[Q43] 标量子查询
来源：http://hz.chenjidiqi.icu/gtjroyyyvk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtpaijwjun.html

[Q44] IN 子查询
来源：http://hz.daxiang520.top/gthxsjewbo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.52xcode.cn/gtvedsmttg.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtoowruiou.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtvkipqjoa.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtxxqulsdy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtckhavvwj.html

[Q47] 与平均值比较
来源：http://hz.snrcjt.cn/gtwxoyjwke.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shangyingyoupin.top/gtbhplpibr.html

[Q48] CTE 公用表表达式
来源：http://hz.kuanghao11.cn/gtarhghlpw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.birdmap.top/gtcoltvldy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gteprgzifx.html

[Q49] 更新单行
来源：http://hz.smart0.xyz/gtedxubilw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fzhhl.top/gtixcgsnod.html

[Q50] 批量更新
来源：http://hz.yueranfly.top/gtgtvfhsmq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.vqdsnc.cn/gtqygcsdzy.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtnoybhzed.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gtbellydkg.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtzpjrwwvo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtubohxnxb.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gtkeiyyfzp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.daria6918.cn/gtpcfeaqht.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gtzraqxmzg.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtkzhsciai.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtpsrhpcxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtogoidzxb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aizwys.cn/gtumoxiclp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gtvkxxekjq.html

[Q57] 行号
来源：http://hz.gzhubu.top/gtfchgneka.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pycfn.com/gthrzhrbda.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtwdfjvxju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtootepzoc.html

[Q59] 分组内累计
来源：http://hz.shzxlz.cn/gtvugpibgm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.0kj1m.cn/gtishusnzy.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtqhttwkpn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sxryk.cn/gtdlmcxjvb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nwbrower.top/gteuemgzwq.html

[Q61] 移动平均
来源：http://hz.guowangkeji.top/gtkitijssh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fengsongda.top/gtpdggjdgk.html

[Q62] 分组占比
来源：http://hz.ivvv.top/gtfrfbcxko.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtrbkoyqfs.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gtqhaokadx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtdmjxyxtp.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtvjbdylre.html

COMMIT;
来源：http://hz.iojbl.cn/gtimldhklo.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtowxtksby.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtxksnvmgt.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtvdjmqpnm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.mhx1999.top/gtfwtimewc.html

[Q67] 设置隔离级别
来源：http://hz.kuanghao11.cn/gtrcsyfvrw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.feifeiyinyue.top/gtjqkqtmgm.html

[Q68] 保存点
来源：http://hz.xuetiantiany.cn/gtcuivefhh.html

SAVEPOINT sp1;
来源：http://hz.yuanzhike.top/gtlzxjtsps.html

ROLLBACK TO sp1;
来源：http://hz.vqdsnc.cn/gtnvwkuoxp.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gthgjnmjqo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258.top/gtdhaioejv.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtlougzyfm.html

ANALYZE TABLE users;
来源：http://hz.xylfe.cn/gteojyozfi.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtgoerxsln.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.svipenyu.cn/gtrbopaary.html

[Q72] 查看索引
来源：http://hz.tanke756.top/gtoyvnhwvf.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtafkzgfwy.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gtzagtkdzy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gzhubu.top/gtcgrlncoi.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtqthssmrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yanxiufei.cn/gtzaapgaog.html

[Q75] 日期格式化
来源：http://hz.gotoacloud.top/gtliqjdvyr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shuidangran.top/gtvlsscjfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinyuanbaomall.cn/gtkojmomyg.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtnzgytrsm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.birdmap.top/gtrnvcsdjj.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtuwhvodfj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gthxfcnvfv.html

[Q78] 当前时间
来源：http://hz.yangfankeji.com/gtlymerrmz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gaohongyu789.top/gtfvwkchju.html

[Q79] 字符串拼接
来源：http://hz.nanxuanxn.top/gtqyqlasfz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258888.top/gtpixpotjk.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gthjjgziim.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtqisuujgc.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtbsosuszk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtxsmqimjv.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gthhgayewm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhongyouzk.top/gtgoxcwieb.html

[Q83] 大小写转换
来源：http://hz.zhoulong.xyz/gtmjuubggk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtnlzucvvk.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtsqmtbgan.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtkjeggvma.html

[Q85] 数值取整
来源：http://hz.jinghuilouyu.cn/gtimwreyhi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tianlin.xyz/gtjpdtvbjo.html

[Q86] 读取 JSON 字段
来源：http://hz.ydzc1.top/gtjkpcqghj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sysykeji.top/gtyeohazii.html

[Q87] JSON 字段做条件
来源：http://hz.jiagoushi.top/gtygcivuqg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sweek.top/gtpotapihc.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtxrxotubh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtixcktqsb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.feifeiyinyue.top/gtobjyjqfj.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gthbfkphgk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtndoyatos.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtsrpvmklw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sweek.top/gtchkeprsv.html

================================================================================
来源：http://hz.svipenyu.cn/gtfrlvpohq.html

R. Bash 专题
来源：http://hz.zdqjudy.top/gtsaomsqei.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthaclqmjz.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtdlviuobd.html

#!/usr/bin/env bash
来源：http://hz.hysaishi.cn/gtjkjbptdh.html

set -euo pipefail
来源：http://hz.chenlongwang.top/gtjkpumevo.html

[R02] 变量赋值与使用
来源：http://hz.yj20258888.top/gtjfclepsl.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtkrscgcfz.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtuwxtwoqh.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtsacbecuy.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtrszbjzod.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.bjfxy.top/gtgmkymjrm.html

[R05] 参数默认值
来源：http://hz.bjfxy.top/gtcudyaeux.html

name="${1:-default}"
来源：http://hz.hysaishi.cn/gtidqrcrfn.html

[R06] 判断命令是否存在
来源：http://hz.wangshuangyany.cn/gtbmnldele.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gttrshugce.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gtanxdxlkz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtfhakxcvk.html

[R08] 数值比较
来源：http://hz.cdnleiting.top/gtdwmntttp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gtckpwfvbm.html

[R09] 字符串比较
来源：http://hz.aibaodan.cn/gtgztluvow.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gttusbjjlv.html

[R10] 正则匹配
来源：http://hz.sufxvd.cn/gtexijbtig.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.meibo888.top/gtgxrribtd.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gttkslxocc.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtkxkuevrs.html

start) echo "启动" ;;
来源：http://hz.chenzaomai.com/gtrfzakyit.html

stop)  echo "停止" ;;
来源：http://hz.snrcjt.cn/gtjwbhuaoy.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gtsoqdzvhg.html

esac
来源：http://hz.jqgfzy.top/gtwnwdnica.html

[R12] for 遍历文件
来源：http://hz.ywan-chungtsiang.top/gtfrlreras.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhijiandao.cn/gthefbmbsr.html

[R13] for 计数循环
来源：http://hz.shangyingyoupin.top/gtreadywnj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yangfankeji.com/gtwyfobzny.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gtlimitvpn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtxyrqlfsd.html

[R15] while 逐行读文件
来源：http://hz.gogol.net.cn/gtnnjjjegk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hammf.cn/gtxjoludxd.html

[R16] until 等待条件
来源：http://hz.tianlin.xyz/gtngcwhaea.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fzhhl.top/gtclaufocg.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtlzveolki.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gthmhufjyc.html

[R18] 遍历数组
来源：http://hz.shzxlz.cn/gtdhgsbqko.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtfcuqlurz.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtmbeekzpi.html

echo "${#arr[@]}"
来源：http://hz.gotoacloud.top/gtxnvksaez.html

[R20] 关联数组（字典）
来源：http://hz.xinyue.icu/gtgpfuipiz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtwppqrtca.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gthsztrmlv.html

echo "${#s}"
来源：http://hz.kuanghao11.cn/gtjodarxml.html

[R22] 截取子串
来源：http://hz.zdqjudy.top/gtatauefqb.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtduvzakae.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gtumvcadyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtxswswidw.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtrjjdknpx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtbriaeehm.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtkjspdmik.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtsvgpwamv.html

[R26] 命令替换
来源：http://hz.gaohongyu789.top/gttdhfitlt.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gtjxuhhtkv.html

[R27] 算术展开
来源：http://hz.jinyuanbaomall.cn/gtyntbvorr.html

echo $((1 + 2 * 3))
来源：http://hz.vqdsnc.cn/gttaorrfqc.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gtqyhsjmrn.html

echo "scale=2; 10/3" | bc
来源：http://hz.yanxiufei.cn/gtedcshcwr.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtblhillgp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtwoifnuqj.html

[R30] 函数返回状态码
来源：http://hz.xinyue.icu/gtyjeklrgy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cqqwz.cn/gtydkyozeq.html

[R31] 局部变量
来源：http://hz.fengsongda.top/gtycjgjqjz.html

f() { local x=1; echo "$x"; }
来源：http://hz.daria6918.cn/gtqprnelbm.html

[R32] 参数个数校验
来源：http://hz.tanke756.top/gtwgkakiuu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gticftplya.html

[R33] 捕获错误并提示行号
来源：http://hz.xuetiantiany.cn/gtppfueyyj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtmjxucujq.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtstsfiwpv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtgtgyyxbz.html

[R35] 后台执行并等待
来源：http://hz.shzxlz.cn/gtskbdxvvu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zycfv.cn/gtpkgsmkfj.html

[R36] 并发执行多个任务
来源：http://hz.cucudq.cn/gtakcobksa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.9152youxi.cn/gtnjovkwvp.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtrcoqhqii.html

files=$(ls -1)
来源：http://hz.cdnleiting.top/gteosmgokj.html

[R38] 管道串联
来源：http://hz.dashuyun.cn/gtlrvbilkr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtvcikvrim.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gthcdhunuh.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gttvolzhal.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtedfgehoi.html

echo "log" >> out.log
来源：http://hz.wangshuangyany.cn/gtqhyxggjt.html

[R41] 丢弃输出
来源：http://hz.meibo888.top/gtjmhgmfhd.html

cmd >/dev/null 2>&1
来源：http://hz.guannengcc.top/gtjkbzvjyo.html

[R42] 输入重定向
来源：http://hz.ydjk.org.cn/gtfzrgmfcw.html

wc -l < a.txt
来源：http://hz.yongpay.top/gtdfbxysxo.html

[R43] 按名字查找文件
来源：http://hz.sxryk.cn/gtvthmpfdo.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtfncpnipj.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtctvxvxay.html

find . -mtime -7 -type f
来源：http://hz.cashguo.top/gtqzxoxiai.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtciaiodgz.html

find . -name "*.tmp" -delete
来源：http://hz.ydzc1.top/gtjhozkein.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gtghgrdmsi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtmoqjrmin.html

[R47] sed 单行替换
来源：http://hz.xylfe.cn/gtvzawkviy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtacrxklid.html

[R48] awk 取指定列
来源：http://hz.zycfv.cn/gtyududter.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtaiurjeqe.html

[R49] awk 带条件
来源：http://hz.316326.xyz/gtwaaxngeg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtmamdnhkj.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtkwsiecni.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtjhysrxhk.html

[R51] 排序去重取前几
来源：http://hz.jqgufenzy.top/gtlexyvmey.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xylfe.cn/gtdcxafadx.html

[R52] 统计行数
来源：http://hz.havefunace.top/gtoqtawzfv.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gtpdgzurem.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtfjcugrbf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydjk.org.cn/gtjhilcvvp.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtuxevykxk.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gttfzzuxev.html

[R55] 压缩与解压
来源：http://hz.chenjidiqi.icu/gtmjlsmstd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtxhhjkzca.html

[R56] 远程拷贝
来源：http://hz.wangdashe.top/gtseqbwauf.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gteqwetxgc.html

[R57] 远程执行命令
来源：http://hz.cqqwz.cn/gtoiqoacvg.html

ssh user@host 'uptime'
来源：http://hz.wangdashe.top/gtjxqdzesk.html

[R58] 下载文件
来源：http://hz.guannengcc.top/gtknftxwcz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gtfhsuudog.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtywrvudmc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtebqlmcah.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtqsigudjr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtfdmiscvh.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtfzgvnesx.html

df -h;  du -sh *
来源：http://hz.yongpay.top/gtdfwhmmaz.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtckqaouul.html

du -ah . | sort -rh | head -10
来源：http://hz.gotoacloud.top/gtcfcfceye.html

[R63] 内存与进程
来源：http://hz.svipenyu.cn/gtepmsqkof.html

free -h;  ps aux | grep nginx
来源：http://hz.yanxiufei.cn/gtjdtjcwwj.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtngxqcnlg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guannengcc.top/gtysjeoyiw.html

[R65] 查看端口占用
来源：http://hz.jqgufenzy.top/gtphvqjpna.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtmgteurcv.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtxsxmcnwy.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtcanxbsbv.html

[R67] 生成随机十六进制串
来源：http://hz.daria6918.cn/gtrfosetrk.html


<!-- 参考信息 -->