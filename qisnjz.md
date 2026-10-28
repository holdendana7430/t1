代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gthhdlhjzg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtqpxzytta.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hnxiangtu.top/gtryzoxjge.html

[Q15] 查询全部
来源：http://hz.zdqjudy.top/gtgkciiqfz.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gtdxydnlst.html

[Q16] 查询指定列
来源：http://hz.chenlongwang.top/gtlxvmcovn.html

SELECT id, name FROM users;
来源：http://hz.jianghu66.top/gtnintkdui.html

[Q17] 条件查询
来源：http://hz.hnqzz.top/gtuaecgcro.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.c1oappe.top/gtbjssizar.html

[Q18] 模糊匹配
来源：http://hz.jiagoushi.top/gtpofnkyjw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhijiandao.cn/gtzhwkwgrg.html

[Q19] 范围查询
来源：http://hz.daxiang520.top/gtilzuayet.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ywan-chungtsiang.top/gtmxntcfcq.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gthwvjjzss.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gthxidzewn.html

[Q21] 空值判断
来源：http://hz.tanke756.top/gtfabxqbaa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.svipenyu.cn/gtjscsepin.html

[Q22] 排序
来源：http://hz.jinyuanbaomall.cn/gtzkzagfka.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jianghu66.top/gtrmxiitbh.html

[Q23] 分页
来源：http://hz.yonumen.top/gtxxinhcex.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhixingplan.top/gtsmtajgdd.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtexqzcspi.html

SELECT DISTINCT city FROM users;
来源：http://hz.hysaishi.cn/gtqhwhjywc.html

[Q25] 只取前 N 条
来源：http://hz.jinqigufen.top/gteavubhyp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sxryk.cn/gtqpcehrwi.html

[Q26] 计数
来源：http://hz.zhaomingkeji.xyz/gtirjgdxek.html

SELECT COUNT(*) FROM users;
来源：http://hz.shuidangran.top/gtxmlohknb.html

[Q27] 条件计数
来源：http://hz.tian-w.cn/gtshazpnof.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cheryme.top/gtulutmerz.html

[Q28] 求和与平均
来源：http://hz.xuanzx.com/gthzdbyktl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.quarkkingdee.top/gtvaxqntxp.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtcedxmnst.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.52xcode.cn/gtfyergbca.html

[Q30] 分组统计
来源：http://hz.ehwqpu.com/gtatlilfqq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtudqiptym.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtoafcwuwi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtgckfmyea.html

[Q32] 分组拼接字符串
来源：http://hz.xylfe.cn/gtxgapdxss.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtuqdxxckb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhijiandao.cn/gtsjfuyiph.html

[Q33] 多列分组
来源：http://hz.haohaochexian.top/gtmxcptyvx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ydjk.org.cn/gtaxfvkalz.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtowtcamkd.html

SELECT * FROM (
来源：http://hz.nanxuanxn.top/gtysektwat.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gtwwxgzaza.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtaevqmpts.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtatsjcxra.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hongshengwenyu.top/gtgkondefv.html

[Q36] 左连接
来源：http://hz.hongshengwenyu.top/gtsrrikqry.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtkpeanvup.html

[Q37] 右连接
来源：http://hz.ybcxt.top/gtwnktqojv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gthdfrtetu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nwbrower.top/gtezvkqxxx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gtoavcidgv.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtfyxmvlpt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gtlchonfhm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sweek.top/gtuautjylg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtsxvzatsj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtdtlxczlx.html

[Q41] 多表连接
来源：http://hz.fzhhl.top/gtqdzdabkd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtokcvhzjl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hammf.cn/gttlafzjil.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gteqpzfpej.html

[Q42] 连接条件附加过滤
来源：http://hz.zhoulong.xyz/gtrrjgxkkx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtbhhknact.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtrvvxflxl.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtoxopazdo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigfzy.top/gtxdytxqhf.html

[Q44] IN 子查询
来源：http://hz.xuanzx.com/gtdywyemat.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yuanzhike.top/gtcyxoifef.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtghdbrlhc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtnqkwjbux.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhaomingkeji.xyz/gtflcfqfiq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtgopitbzv.html

[Q47] 与平均值比较
来源：http://hz.gzhubu.top/gtkpztxjes.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgfzy.top/gtlnshnlcq.html

[Q48] CTE 公用表表达式
来源：http://hz.andypj.xyz/gtikbigjpo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinghuilouyu.cn/gtjyuptaao.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtcilyfums.html

[Q49] 更新单行
来源：http://hz.ydzc1.top/gtlxsvpike.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.andypj.xyz/gtwxnzbuia.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gttwzypuge.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gtftuuzgyc.html

[Q51] 用子查询更新
来源：http://hz.hfpthk.cn/gtafmhedwo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tian-w.cn/gtdwanxfym.html

[Q52] 删除指定行
来源：http://hz.sysykeji.top/gtksexrkgd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtehviqxzi.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtgjmyqhsb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangshuangyany.cn/gtuiyehtsz.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtfydbsjcb.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtkmmbobch.html

[Q55] 排名（并列占位）
来源：http://hz.jqgfzy.top/gtsauiccat.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.aibaodan.cn/gtqtxicjkn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinyuanbaomall.cn/gtutyalzlp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gtjfpgqevi.html

[Q57] 行号
来源：http://hz.zhaomingkeji.xyz/gtwcpgqpye.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangtech.top/gtznbfpird.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gtmknwsvpe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtthplcjag.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtyrfzyngk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jlsjyb.cn/gtjhodrwow.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gttaquxbcd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.snrcjt.cn/gtmswenkan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guannengcc.top/gtrvotdoty.html

[Q61] 移动平均
来源：http://hz.birdmap.top/gtipmzugce.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.fzhhl.top/gtooaqskvq.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gthhivcbmh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtwflkhgqw.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gtcorerurr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gtxueytgnv.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gtfrvpmyjo.html

COMMIT;
来源：http://hz.daria6918.cn/gtkscuwwsj.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtijykddlm.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtruofxdjb.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtufdweyft.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxuanxn.top/gtfkqpxxlf.html

[Q67] 设置隔离级别
来源：http://hz.daxiang520.top/gtjsepsrzp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ivvv.top/gtxlppqwqd.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtahkxyfau.html

SAVEPOINT sp1;
来源：http://hz.hammf.cn/gtybfiryaw.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtnkdpxetq.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtcaorcfaq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtupydqnmt.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtseaoxnmh.html

ANALYZE TABLE users;
来源：http://hz.hammf.cn/gtlfejarvd.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtigrwujys.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtsvnnmejy.html

[Q72] 查看索引
来源：http://hz.yuanzhike.top/gtnxtyxbea.html

SHOW INDEX FROM users;
来源：http://hz.sxryk.cn/gtqowmupje.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtxneljkiy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenlongwang.top/gtrkuurksh.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtejsjuyxt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgufenzy.top/gtxmhsrgew.html

[Q75] 日期格式化
来源：http://hz.redwolf501.top/gtncokjcop.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtitcqtlkm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xuetiantiany.cn/gtxfgrrnrz.html

[Q76] 按天统计
来源：http://hz.shanyushiyangtech.top/gtmgupjbgl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gaohongyu789.top/gtodwqeanz.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtqggfqyia.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.quarkkingdee.top/gtovgryqdb.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gtyjkdnmmf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtozhpgpth.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gtbmytodvy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ivvv.top/gtzttivfjs.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gthzapkcqm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj20258.top/gtqkowjscf.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtjkbrcjxr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhongyouzk.top/gtxvqpspth.html

[Q82] 字符长度与字节长度
来源：http://hz.meibo888.top/gtjgbnovtg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtrhhkntug.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gtpkkxkwqv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cdnleiting.top/gtrrxjrpel.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtthnifenp.html

SELECT TRIM(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtpvssmwru.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtttjmtqjr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtnltgyzyw.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtzcwhankj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zdqjudy.top/gtilwjuugj.html

[Q87] JSON 字段做条件
来源：http://hz.iojbl.cn/gtxlhdqqfz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yanxiufei.cn/gtejqlmser.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtlkbpxnzy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtggkxntqu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtnaqadbip.html

[Q89] 判断表是否存在
来源：http://hz.hnxiangtu.top/gtbbbupgrj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtydpcedox.html

[Q90] 生成序号列
来源：http://hz.hnqzz.top/gttjjhbklz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.c1oappe.top/gtceuejnxx.html

================================================================================
来源：http://hz.52xcode.cn/gtuqkilylc.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtekwumcpy.html

================================================================================
来源：http://hz.yvedp.cn/gtwqezxlyr.html

[R01] shebang 与严格模式
来源：http://hz.hysaishi.cn/gthmeapisu.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtdbhzfjsd.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtymhfyfyk.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtwpfgcubm.html

name="Tom"; echo "$name"
来源：http://hz.gotoacloud.top/gtqchudcin.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gtztnjkupz.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtwtnggjdp.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gthbvwgtil.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtuwugykfy.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtwavdtfqf.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtbufyxikc.html

[R06] 判断命令是否存在
来源：http://hz.svipenyu.cn/gtoyyjfwds.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sysykeji.top/gtlssunntd.html

[R07] if 判断文件
来源：http://hz.zhoulong.xyz/gtwkwfzpjs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtitgsqwkr.html

[R08] 数值比较
来源：http://hz.zhiwuduotai.top/gtsibgckjj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gthvbfwnpg.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtfjvqdgic.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhoulong.xyz/gtyyntbjem.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtfwfcchwn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yvedp.cn/gtesxuvqyg.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtfbfeuvxh.html

case "$1" in
来源：http://hz.yonumen.top/gtmrexbqwm.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtuchbiqyu.html

stop)  echo "停止" ;;
来源：http://hz.sxryk.cn/gtgeoednyp.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gtesuosojh.html

esac
来源：http://hz.haohaochexian.top/gttcofpumt.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtyuvzjamd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gtpohanxpg.html

[R13] for 计数循环
来源：http://hz.zhiwuduotai.top/gtyeqhhubr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.birdmap.top/gtexuywygk.html

[R14] C 风格 for
来源：http://hz.tian-w.cn/gtxlzqpazf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxinkj.top/gtatsrbgik.html

[R15] while 逐行读文件
来源：http://hz.nwbrower.top/gtozeywesh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtesiypwsf.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtulfoqhqj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtvztxmhdn.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtzcqduabb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cheryme.top/gtyuczwlas.html

[R18] 遍历数组
来源：http://hz.daria6918.cn/gtcslecuig.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhiwuduotai.top/gttrbxfnzg.html

[R19] 数组长度
来源：http://hz.vqdsnc.cn/gtsdczjwhm.html

echo "${#arr[@]}"
来源：http://hz.zhijiandao.cn/gtbonilnqs.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtshwpqetx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtmgfzcpwl.html

[R21] 字符串长度
来源：http://hz.jyoumei.cn/gtysuyhesy.html

echo "${#s}"
来源：http://hz.jinqigfzy.top/gtgsjiwbne.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtjvzsbecm.html

echo "${s:0:5}"
来源：http://hz.gaohongyu789.top/gtcokfcoct.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gtpzbqktgu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtvbhlrkbj.html

[R24] 大小写转换
来源：http://hz.guannengcc.top/gtrwmhsoky.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtvwyiwwlc.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtcvdxutbp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tanke756.top/gtnkwwsgig.html

[R26] 命令替换
来源：http://hz.gaohongyu789.top/gttckhuyej.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtbbrjvgtu.html

[R27] 算术展开
来源：http://hz.dashuyun.cn/gtqfaioaqz.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gttnsrhriq.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtnfeifgtv.html

echo "scale=2; 10/3" | bc
来源：http://hz.jqgufenzy.top/gtpssxyiym.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtjprprfpb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zdqjudy.top/gtaiqjckvv.html

[R30] 函数返回状态码
来源：http://hz.c1oappe.top/gtcwdudtlx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtalquioqp.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gthhiaappg.html

f() { local x=1; echo "$x"; }
来源：http://hz.haohaochexian.top/gtnalngafg.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gttnktfcqc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtmgjrozim.html

[R33] 捕获错误并提示行号
来源：http://hz.fzhhl.top/gtgotuyuxg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtxthvtlay.html

[R34] 退出时清理
来源：http://hz.9152youxi.cn/gtasogodpq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtwysmeami.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtwgxljyhq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guowangkeji.top/gtezfwmfbj.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtchflcols.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hysaishi.cn/gtvzflfjpw.html

[R37] 把输出赋给变量
来源：http://hz.daria6918.cn/gtvhlxjjmn.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtktyctqtx.html

[R38] 管道串联
来源：http://hz.daria6918.cn/gthgpelymz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtfflnmmzw.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gtwyfblygg.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtppsgfagb.html

[R40] 追加写日志
来源：http://hz.sweek.top/gtpejyzyrh.html

echo "log" >> out.log
来源：http://hz.mhx1999.top/gtstcpoosg.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtmhmhcblb.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gtdesvnthe.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtojgusmuf.html

wc -l < a.txt
来源：http://hz.gzhubu.top/gtcoyeimxf.html

[R43] 按名字查找文件
来源：http://hz.nanxinkj.top/gtunqdhclq.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtyaovzpez.html

[R44] 按修改时间查找
来源：http://hz.guowangkeji.top/gtetmobzuc.html

find . -mtime -7 -type f
来源：http://hz.bjfxy.top/gtwewnxzzq.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtzsenotlc.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigufen.top/gtahdpjhvt.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtmkptaqbo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gtfdphktzb.html

[R47] sed 单行替换
来源：http://hz.hongshengwenyu.top/gtxrgrihuz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtwxadzkpr.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtuabtfwpz.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuanzx.com/gtvoywamay.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtblyzppfl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xinyue.icu/gtdvyiolib.html

[R50] awk 求和
来源：http://hz.yueranfly.top/gtszupykcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.9152youxi.cn/gtibrzaref.html

[R51] 排序去重取前几
来源：http://hz.9152youxi.cn/gtyjkvtqsc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtffwvvvan.html

[R52] 统计行数
来源：http://hz.mhx1999.top/gtntalrihk.html

wc -l a.txt
来源：http://hz.sweek.top/gtfpneismp.html

[R53] 查看文件头与实时尾
来源：http://hz.yueranfly.top/gthiybsqja.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydzc1.top/gtkstopsqc.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtgjbqjeoe.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtlojvbhkj.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gtxjutmktd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ybcxt.top/gtdxcsakcu.html

[R56] 远程拷贝
来源：http://hz.haohaochexian.top/gttqgusysj.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtrseketeg.html

[R57] 远程执行命令
来源：http://hz.shzxlz.cn/gtfskglvna.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtogcnnaka.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtfkrxmblp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtpmmzdpwc.html

[R59] 发 POST JSON
来源：http://hz.ehwqpu.com/gtbwljgzzb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jiagoushi.top/gtbxvronor.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gtmpgksuvt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuetiantiany.cn/gtpoptxlpl.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtmczgtdmq.html

df -h;  du -sh *
来源：http://hz.zhengqikj.top/gtyszfluvw.html

[R62] 找最占空间的文件
来源：http://hz.vqdsnc.cn/gtnmhoxhdf.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgfzy.top/gtcpxtndfv.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gtgeclxcqy.html


<!-- 参考信息 -->