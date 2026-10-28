代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gtfsfavrux.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtqyrslgot.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtosemvpli.html

[Q21] 空值判断
来源：http://hz.sweek.top/gtecobfolk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtwrqjflpq.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtinorsgra.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gtqzxyneeu.html

[Q23] 分页
来源：http://hz.meibo888.top/gtowrzwevn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shzxlz.cn/gtkelzuxfe.html

[Q24] 去重
来源：http://hz.daria6918.cn/gtazlycgdh.html

SELECT DISTINCT city FROM users;
来源：http://hz.guannengcc.top/gtmdtotfid.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtteaiemgm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.316326.xyz/gtlknpabbo.html

[Q26] 计数
来源：http://hz.daria6918.cn/gtwljbktfi.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydzc1.top/gtulsuufou.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtydmwgkaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gtnndfrvrn.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtusupljns.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtkgrzbndl.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtxhepgfvq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtirpgwikx.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtprribzud.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gturoohujt.html

[Q31] 分组后过滤
来源：http://hz.dianchejie.cn/gtahfselxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtkvvnnzhx.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtgqcevfdx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtalwerpzi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhengqikj.top/gtuuqzpshh.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtaciolirs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhijiandao.cn/gtjjiocoui.html

[Q34] 每组取第一条
来源：http://hz.316326.xyz/gtvdynuhti.html

SELECT * FROM (
来源：http://hz.ydzc1.top/gtaeynpnrq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhixingplan.top/gtzarrjbug.html

) t WHERE rn = 1;
来源：http://hz.wangdashe.top/gtxuexuaam.html

[Q35] 内连接
来源：http://hz.ydjk.org.cn/gterbmrcit.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtmashqkzv.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtmdlllvfj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtpbaeqlkl.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtqeqixras.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtfpnvmpsu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tianlin.xyz/gtgndyrcfc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.wangshuangyany.cn/gtgqpyodci.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtrumxdjzm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtxsbpqrzw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtwyprytox.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shuidangran.top/gtkxyfeebr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tianlin.xyz/gtztfwgdgw.html

[Q41] 多表连接
来源：http://hz.dianchejie.cn/gtzltngtxs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.meibo888.top/gtlxtfmlas.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtcoslqpzw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xingfuxueyuan.xyz/gtjyxptfot.html

[Q42] 连接条件附加过滤
来源：http://hz.yueranfly.top/gtaqpkmliy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ydjk.org.cn/gtgrxauwga.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydjk.org.cn/gthadvhlyj.html

[Q43] 标量子查询
来源：http://hz.yueranfly.top/gtyzdhnuwk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtnudssygk.html

[Q44] IN 子查询
来源：http://hz.xinyue.icu/gtucqylvud.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.pengpengdd.cyou/gtkxprofdh.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gtchxqqugl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gthvgnfqcj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtkdptyhbn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtsmvwnall.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtniedfqce.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gzhubu.top/gtmbzvkhph.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxuanxn.top/gtbymgtnls.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.birdmap.top/gtomzgzgmv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhengqikj.top/gtzsuomqde.html

[Q49] 更新单行
来源：http://hz.feifeiyinyue.top/gthmdcfwpl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cashguo.top/gtrifmcomu.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtvpdmpqgm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.9152youxi.cn/gtvekanljh.html

[Q51] 用子查询更新
来源：http://hz.zhijiandao.cn/gtyjvgoxty.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tianlin.xyz/gteexyarip.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gtgtvccufg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtserooxsa.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtvidojscm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.feifeiyinyue.top/gtvbpyzfbu.html

[Q54] 清空表
来源：http://hz.yongpay.top/gtfencrqys.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtgqqmclli.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gtrahkkvnn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gthuwymzak.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhongyouzk.top/gtbdrcmdjz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gtdiwpzftu.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtcgrdfjfd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gogol.net.cn/gtiqbglobk.html

[Q58] 累计求和
来源：http://hz.sysykeji.top/gtcsqgzwkj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtidvqcqsx.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtanryzvvt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gthedsxico.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtuooynccd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtzvseozog.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xinyue.icu/gtusyugodz.html

[Q61] 移动平均
来源：http://hz.dashuyun.cn/gtsbhtaqbs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtvabgmmrp.html

[Q62] 分组占比
来源：http://hz.zhiwuduotai.top/gtfdizcrxq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtqzbnyqrz.html

[Q63] 开启事务
来源：http://hz.ydjk.org.cn/gtfnmcmfuo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.guannengcc.top/gtnnmciyyh.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gtkubsbcyu.html

COMMIT;
来源：http://hz.andypj.xyz/gttstgogwl.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtjxbcbcmj.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtfadxzzmk.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtnnaxkekr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gttcecxdev.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtuckuyvcx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtwvnrgnsi.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtgfofmokg.html

SAVEPOINT sp1;
来源：http://hz.zhijiandao.cn/gtciiiszoq.html

ROLLBACK TO sp1;
来源：http://hz.jinqigfzy.top/gtuqqxkzrh.html

[Q69] 查看执行计划
来源：http://hz.9152youxi.cn/gtjxqzidbt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhongyouzk.top/gtnmflrxyt.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtypuhpvmw.html

ANALYZE TABLE users;
来源：http://hz.gogol.net.cn/gtbnmvasue.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gtcrcfyfcb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtbnfldhaf.html

[Q72] 查看索引
来源：http://hz.zhiwuduotai.top/gtefxsppqt.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gthbibmikj.html

[Q73] 查看表状态
来源：http://hz.jlsjyb.cn/gtrgtxyoyi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtfxbvqegg.html

[Q74] 强制使用索引
来源：http://hz.yonumen.top/gtezlazrni.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gotoacloud.top/gtcedbkbve.html

[Q75] 日期格式化
来源：http://hz.xuanzx.com/gtjdnmczdy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj20258.top/gtzisagjwc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtgdgwljfa.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtrjojszjf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zdqjudy.top/gtafmpcesk.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gthfjivuvl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cheryme.top/gtgthjqaat.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gthmdtepzc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cucudq.cn/gtbndcqnrl.html

[Q79] 字符串拼接
来源：http://hz.sweek.top/gtieutvjhn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aibaodan.cn/gtkhcaqxgd.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtccedipdf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jianghu66.top/gtuxkzqdrg.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gtlehertgi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.wangdashe.top/gtqpxzrkyo.html

[Q82] 字符长度与字节长度
来源：http://hz.guannengcc.top/gtsntxgmwh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gotoacloud.top/gtdsqfmlbl.html

[Q83] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtocbskbwy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtyfuksbex.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangtech.top/gtuffpbcme.html

SELECT TRIM(name) FROM users;
来源：http://hz.jqgfzy.top/gtxuxldrrk.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtuxehkzwt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtyxmgekve.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtkotbkdxm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtecpgqutq.html

[Q87] JSON 字段做条件
来源：http://hz.guowangkeji.top/gtxiprkcvh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtqauqczop.html

[Q88] 行转列（条件聚合）
来源：http://hz.sweek.top/gtkmamcmhf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtgdtbqlxe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuxming.cn/gtrpxidruf.html

[Q89] 判断表是否存在
来源：http://hz.svipenyu.cn/gtmcebpwrd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtowlqujlr.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtevncxojo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guannengcc.top/gtwlonxcnq.html

================================================================================
来源：http://hz.cashguo.top/gtbforjsyu.html

R. Bash 专题
来源：http://hz.yj20258.top/gtpmxuqhyg.html

================================================================================
来源：http://hz.mhx1999.top/gtakmjeikx.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtezlkbxks.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtssonkabh.html

set -euo pipefail
来源：http://hz.ydjk.org.cn/gtbipxvfbh.html

[R02] 变量赋值与使用
来源：http://hz.jinqigfzy.top/gtmciwfkiv.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gtzcrgofxk.html

[R03] 只读变量
来源：http://hz.jinqigufen.top/gtfvxpwouj.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtnrgyffsn.html

[R04] 位置参数
来源：http://hz.aizwys.cn/gtxrshhrfn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtayautvxj.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtocjyekqj.html

name="${1:-default}"
来源：http://hz.chenjidiqi.icu/gtyjkznnmx.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtoworkrbe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtkofziouf.html

[R07] if 判断文件
来源：http://hz.52xcode.cn/gtqpghbtal.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtwhruecmu.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gtrgikzxhv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtrugjqutn.html

[R09] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtngiwpppf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aibaodan.cn/gtyufppcdl.html

[R10] 正则匹配
来源：http://hz.dashuyun.cn/gtvvzlilmh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zdqjudy.top/gtbyolelip.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtqrbzskgy.html

case "$1" in
来源：http://hz.wangshuangyany.cn/gtztliprir.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtkovcnytx.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtfouocvar.html

*)     echo "未知命令" ;;
来源：http://hz.ydjk.org.cn/gtlglrywak.html

esac
来源：http://hz.jinyuanbaomall.cn/gtjzhrzpjk.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtpcpewgru.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fengsongda.top/gtneplhzue.html

[R13] for 计数循环
来源：http://hz.yuxming.cn/gtomzdqtdf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gtrmfqyfcm.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtdqvuoopn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtdwabvyko.html

[R15] while 逐行读文件
来源：http://hz.wangdashe.top/gtevcipmop.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtfitdsiba.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gteduhywtn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtpkpnoqkv.html

[R17] 数组定义与取值
来源：http://hz.hysaishi.cn/gtsmorhfsy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.9152youxi.cn/gtbkgyihlj.html

[R18] 遍历数组
来源：http://hz.zhiwuduotai.top/gtntzgyywc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gtacgdmkcm.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gthbmpmjqz.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gtkmtodwcs.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gtviaxtpkv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtzrmtuokc.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtnxsrhlyp.html

echo "${#s}"
来源：http://hz.c1oappe.top/gtujuermus.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtwnewtuum.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtwidsjzsm.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtvcoviwgh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtuvqecfod.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtpylkxwrq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gtlmizgdjw.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtjpnjnonp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pengpengdd.cyou/gthhmqmkbv.html

[R26] 命令替换
来源：http://hz.tianlin.xyz/gtjouqjfjd.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gtqlnfghiw.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtmqedkcid.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtreqasllr.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtnjnfctdo.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtpykohekf.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtkdzlajyc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtfnenvihr.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtrgfeolpj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hysaishi.cn/gtxlmfefau.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtkzixptfq.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtltrcwhyd.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtamqgilzi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.9152youxi.cn/gtekenxzry.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gttdbwgtot.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuanzhike.top/gtnstkktvy.html

[R34] 退出时清理
来源：http://hz.guannengcc.top/gtxwrbriqo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtotrasxxs.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gtolrzrxbg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gaohongyu789.top/gtqysconkt.html

[R36] 并发执行多个任务
来源：http://hz.zhijiandao.cn/gtufqnodga.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guowangkeji.top/gtkkzwbbuo.html

[R37] 把输出赋给变量
来源：http://hz.shuidangran.top/gtsyzmrpnh.html

files=$(ls -1)
来源：http://hz.wangdashe.top/gtkfkchkun.html

[R38] 管道串联
来源：http://hz.yj20258888.top/gtqjgfsoif.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jianghu66.top/gtjmoyrcoc.html

[R39] 重定向标准输出与错误
来源：http://hz.zdqjudy.top/gtwvuypdts.html

cmd > out.log 2>&1
来源：http://hz.haohaochexian.top/gtescfuiod.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtgpchxnbp.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtdogjonva.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtqlhomjjm.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtmwyoxuya.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtyspqjisp.html

wc -l < a.txt
来源：http://hz.52xcode.cn/gtycbhuxfn.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtpkpdopqg.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtaoqthuio.html

[R44] 按修改时间查找
来源：http://hz.pycfn.com/gtvvciwpxc.html

find . -mtime -7 -type f
来源：http://hz.zhijiandao.cn/gtvlwvuydl.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtvlwaomii.html

find . -name "*.tmp" -delete
来源：http://hz.gaohongyu789.top/gtfzeuqhpm.html

[R46] 递归替换文件内容
来源：http://hz.aizwys.cn/gtgvoujkfq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.feifeiyinyue.top/gtcpluavsm.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gtgicirdqo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtiqggmgqy.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtqjapeerq.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinghuilouyu.cn/gtoxqydeii.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gteyntebqn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtwbeyhcvc.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtysgbczjh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yanxiufei.cn/gtlmjlymof.html

[R51] 排序去重取前几
来源：http://hz.feifeiyinyue.top/gtohtmiaxj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yanxiufei.cn/gtwhdftqfq.html

[R52] 统计行数
来源：http://hz.guannengcc.top/gtzkqidpli.html

wc -l a.txt
来源：http://hz.nwbrower.top/gtrfhqdpfg.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtvrumzlnj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hammf.cn/gtdmxrrqzy.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gtqzibmsnd.html

diff a.txt b.txt
来源：http://hz.svipenyu.cn/gtjqwuudvr.html

[R55] 压缩与解压
来源：http://hz.hongshengwenyu.top/gtuhcoiekc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinyuanbaomall.cn/gtsgowsdss.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangtech.top/gtrqdpradx.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtllfeleok.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtpbcytxfu.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtvsamdyac.html

[R58] 下载文件
来源：http://hz.fzhhl.top/gtyhuzsqep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.316326.xyz/gtmtafrfgw.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtuenlaoht.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yonumen.top/gtaqttirdg.html

[R60] 只看 HTTP 状态码
来源：http://hz.pycfn.com/gtmeskwoae.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj20258.top/gtlvafclpx.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtlrithguc.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gteddoehsb.html

[R62] 找最占空间的文件
来源：http://hz.jinqigfzy.top/gtmgvdmaou.html

du -ah . | sort -rh | head -10
来源：http://hz.redwolf501.top/gtzyzuitlo.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtbgzndwcq.html

free -h;  ps aux | grep nginx
来源：http://hz.ehwqpu.com/gtjvxbdmmh.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtqzbxcban.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtvmpljsvt.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtfiifpgyw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhixingplan.top/gtshczsazu.html

[R66] 定时任务
来源：http://hz.hysaishi.cn/gtfmgdrphc.html

crontab -e;  crontab -l
来源：http://hz.vqdsnc.cn/gtpvulszqi.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtnbvzlchi.html

openssl rand -hex 16
来源：http://hz.gotoacloud.top/gtdmedpajh.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtnbdijzwh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtlmaompxa.html

[R69] 生成随机密码
来源：http://hz.316326.xyz/gtnsfuwfjf.html


<!-- 参考信息 -->