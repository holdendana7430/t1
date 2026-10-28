代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.quarkkingdee.top/gtnlgqojgy.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangtech.top/gthkzftcoi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jianghu66.top/gtqknamxql.html

[Q19] 范围查询
来源：http://hz.sweek.top/gtmistivwy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fengsongda.top/gtvfdckdmw.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtdcfzfnmz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtpipfrgtf.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtvrwwypmy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258.top/gtdfjvihcz.html

[Q22] 排序
来源：http://hz.svipenyu.cn/gtrvhjspyp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtzxbmzyea.html

[Q23] 分页
来源：http://hz.hnqzz.top/gtkyeqndza.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aizwys.cn/gtptswmeue.html

[Q24] 去重
来源：http://hz.hammf.cn/gtbfbipwza.html

SELECT DISTINCT city FROM users;
来源：http://hz.jianghu66.top/gtfzyeonru.html

[Q25] 只取前 N 条
来源：http://hz.shuidangran.top/gtrdsrltuf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shanyushiyangkeji.top/gtaqpyhptl.html

[Q26] 计数
来源：http://hz.hammf.cn/gtudhkilgj.html

SELECT COUNT(*) FROM users;
来源：http://hz.yvedp.cn/gtchxtijvb.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtfpqlccso.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fzhhl.top/gtqbrlqvte.html

[Q28] 求和与平均
来源：http://hz.redwolf501.top/gtizncrnje.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhixingplan.top/gthfwfqepo.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtspgratel.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gttmmeuqez.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtxpjupdiq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtdcyplgiz.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtcxwpxogn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtoaeszzxg.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtimrsctjn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtwimjaegu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtscudprzf.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gtooizkgte.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtlfzylmwj.html

[Q34] 每组取第一条
来源：http://hz.havefunace.top/gtbkbkkvnz.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtxigfoiyd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jianghu66.top/gtcerapixs.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtujmhtftl.html

[Q35] 内连接
来源：http://hz.kuanghao11.cn/gtgarismou.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtqvwlogiy.html

[Q36] 左连接
来源：http://hz.xziqi.cn/gtzmltmrpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhiwuduotai.top/gtouhreepf.html

[Q37] 右连接
来源：http://hz.zhiwuduotai.top/gtsqazqina.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhaomingkeji.xyz/gtxdohizjp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhixingplan.top/gtruwzqjxg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtliynwlfk.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtkkkkqzug.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.0kj1m.cn/gttccphbdo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtlxyowryj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.havefunace.top/gtuxvvbsim.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.meibo888.top/gthpwwfliz.html

[Q41] 多表连接
来源：http://hz.tanke756.top/gtwimogdeb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gotoacloud.top/gtsmgvvwjx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zycfv.cn/gtmggdlvkg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sysykeji.top/gtpsyzlqzv.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtwebordfp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hnxiangtu.top/gtccnkpahu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtxtgmhezz.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtipucldfw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtxhljltye.html

[Q44] IN 子查询
来源：http://hz.zycfv.cn/gtvwdxhfzy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangdashe.top/gtjbkneffi.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtbudxgepy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtwarutfse.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtrylbpjvz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtrzurlatf.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gthqwtdbxl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zycfv.cn/gttqnyxwyz.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtpoakmrhl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtniuosxmc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hongshengwenyu.top/gtnqpspkkd.html

[Q49] 更新单行
来源：http://hz.52xcode.cn/gtqnnscmjl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtkntizzav.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtsibzinfm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtpnamlxmj.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtlrhdtjzl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gtdagiqxtu.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtbscqwbyd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtizdxuhdl.html

[Q53] 按条件删除
来源：http://hz.xinyue.icu/gteevmmquc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sysykeji.top/gtqauimuez.html

[Q54] 清空表
来源：http://hz.sweek.top/gtqitrncih.html

TRUNCATE TABLE logs;
来源：http://hz.cashguo.top/gtmdufspqh.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangkeji.top/gtkwechseh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gzhubu.top/gtfkvltwgi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xylfe.cn/gtopdkkkyv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigfzy.top/gtdtcpdxuz.html

[Q57] 行号
来源：http://hz.kuanghao11.cn/gtczgvisay.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shuidangran.top/gtqbctzzck.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtnnszkwog.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jiagoushi.top/gtndxgfmmo.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtfhyjuqdx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxinkj.top/gtfdiqqqzl.html

[Q60] 取上一行 / 下一行
来源：http://hz.xziqi.cn/gtohbfovls.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtxokayvcm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.c1oappe.top/gtnxdshmzn.html

[Q61] 移动平均
来源：http://hz.hywenlv.cn/gtfcqqgmtt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shuidangran.top/gtieblhrlf.html

[Q62] 分组占比
来源：http://hz.hongshengwenyu.top/gtmfczmhjy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtjqkwuflu.html

[Q63] 开启事务
来源：http://hz.ydzc1.top/gtbpnmcymn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gzhubu.top/gtvfwwgvbq.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtkvatghdu.html

COMMIT;
来源：http://hz.aizwys.cn/gtksgemzvw.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtkxsaclam.html

ROLLBACK;
来源：http://hz.wangshuangyany.cn/gtemhpvjtl.html

[Q66] 行锁查询
来源：http://hz.yanxiufei.cn/gtxikfumnc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.quarkkingdee.top/gtsfcnbvgf.html

[Q67] 设置隔离级别
来源：http://hz.smart0.xyz/gtyezaysxg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gzhubu.top/gtxwbttati.html

[Q68] 保存点
来源：http://hz.xuanzx.com/gtqpwmnxdc.html

SAVEPOINT sp1;
来源：http://hz.sxryk.cn/gtqaqpgcha.html

ROLLBACK TO sp1;
来源：http://hz.ehwqpu.com/gtwqvncazr.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtooynchsk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yueranfly.top/gtymzqwale.html

[Q70] 更新统计信息
来源：http://hz.cqqwz.cn/gtwmmizozq.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gtxccauwgl.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtxsawtjhh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gttktndaje.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtlygevgbm.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtwzivhvym.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gtsmwhizjk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenzaomai.com/gtarezatcb.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtmvrorjdd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenzaomai.com/gtmedjdsrm.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtkqmbwjfm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtzeubffpi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinyuanbaomall.cn/gtwpzbzjnd.html

[Q76] 按天统计
来源：http://hz.0kj1m.cn/gtbbxlbmyx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guannengcc.top/gtrkhqeisz.html

[Q77] 时间加减
来源：http://hz.jinghuilouyu.cn/gtlzorblbl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtxkthwxpl.html

[Q78] 当前时间
来源：http://hz.hysaishi.cn/gtvhiplqpu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxuanxn.top/gtqwidcwfq.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtwtbwlbuc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cheryme.top/gtggoamhmj.html

[Q80] 字符串截取
来源：http://hz.pengpengdd.cyou/gtblhvtcpt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuanzx.com/gthifpmbms.html

[Q81] 字符串替换
来源：http://hz.haohaochexian.top/gtiaflzops.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtkzddnzfm.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtvceukwnz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtpdwxdtcx.html

[Q83] 大小写转换
来源：http://hz.meibo888.top/gtxzqgxklw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtsjubczbb.html

[Q84] 去除首尾空格
来源：http://hz.hywenlv.cn/gtivihabye.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtioloaiyt.html

[Q85] 数值取整
来源：http://hz.xingfuxueyuan.xyz/gtghusldli.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jiagoushi.top/gtfcbiunoi.html

[Q86] 读取 JSON 字段
来源：http://hz.ppjwa.cn/gtajbnnune.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtrwlzsgmj.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258.top/gtxrgwddop.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cdnleiting.top/gttaajhfjj.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtmtsveqjg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtvzefmxoh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtdbetqlhd.html

[Q89] 判断表是否存在
来源：http://hz.9152youxi.cn/gtxnwuzaqk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtswjwicpl.html

[Q90] 生成序号列
来源：http://hz.feifeiyinyue.top/gtcvsgixiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtrrivfdyf.html

================================================================================
来源：http://hz.xylfe.cn/gtcqimcvwx.html

R. Bash 专题
来源：http://hz.shangyingyoupin.top/gtpqgzjwun.html

================================================================================
来源：http://hz.hnxiangtu.top/gttcmiajub.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtoodkkgnd.html

#!/usr/bin/env bash
来源：http://hz.hfpthk.cn/gtvfgihlig.html

set -euo pipefail
来源：http://hz.sufxvd.cn/gtspbdzunw.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtjuhmhxgw.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtumuaztrq.html

[R03] 只读变量
来源：http://hz.zhixingplan.top/gtxrklmkun.html

readonly PI=3.14
来源：http://hz.yonumen.top/gtlmkrvgut.html

[R04] 位置参数
来源：http://hz.cqqwz.cn/gtpwertbit.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtxnrcywaw.html

[R05] 参数默认值
来源：http://hz.jqgfzy.top/gtjaoiihpw.html

name="${1:-default}"
来源：http://hz.jinqigfzy.top/gtyfjamfti.html

[R06] 判断命令是否存在
来源：http://hz.nanxinkj.top/gtnefwvpju.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jlsjyb.cn/gtfnqgovqs.html

[R07] if 判断文件
来源：http://hz.sweek.top/gtkgodjjll.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinyuanbaomall.cn/gtjguduuxf.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtosvgfdji.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gtkvisblqj.html

[R09] 字符串比较
来源：http://hz.sufxvd.cn/gtmyyojuxv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hysaishi.cn/gttqjuejti.html

[R10] 正则匹配
来源：http://hz.52xcode.cn/gtxwtemfto.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pycfn.com/gtewrigkdf.html

[R11] case 多分支
来源：http://hz.hfpthk.cn/gtnwjmstut.html

case "$1" in
来源：http://hz.chenlongwang.top/gtznubuijc.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gtwzqqoogf.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gttbsqqpie.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gthyiraczv.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtlycougqt.html

[R12] for 遍历文件
来源：http://hz.feifeiyinyue.top/gtclefpirq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinghuilouyu.cn/gtzgxvlyhy.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtkxsrsidr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtrrifexud.html

[R14] C 风格 for
来源：http://hz.smart0.xyz/gtxxdqbfwq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtvrvbrjjt.html

[R15] while 逐行读文件
来源：http://hz.gotoacloud.top/gtssmuegyp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtbyueqrhy.html

[R16] until 等待条件
来源：http://hz.xuanzx.com/gtdpuhtlgf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gtsxmujktv.html

[R17] 数组定义与取值
来源：http://hz.shangyingyoupin.top/gtbspszrev.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.kuanghao11.cn/gtuhgdenkp.html

[R18] 遍历数组
来源：http://hz.gaohongyu789.top/gtkhvrcccw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtupkwldci.html

[R19] 数组长度
来源：http://hz.jlsjyb.cn/gtynddzpwn.html

echo "${#arr[@]}"
来源：http://hz.jqgufenzy.top/gthlcvvzkj.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtqtexpihe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuanzx.com/gtugjmttfw.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtgwoldmmr.html

echo "${#s}"
来源：http://hz.redwolf501.top/gtfqlcepxe.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtdvdaxbhv.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gtyslpviaw.html

[R23] 字符串替换
来源：http://hz.iojbl.cn/gtapfcqdet.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gttqdvworx.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtxnojpyod.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.c1oappe.top/gtaeyifvui.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuanzhike.top/gtoqjihngy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtisuntwbf.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtiozezsfr.html

now=$(date +%F); echo "$now"
来源：http://hz.fzhhl.top/gtbyzqjwtz.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gteduftkcz.html

echo $((1 + 2 * 3))
来源：http://hz.ydzc1.top/gtwljjsjlo.html

[R28] 浮点运算
来源：http://hz.hysaishi.cn/gttsgzrpju.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtqtlrhhqa.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtxneiscxb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtgzlrvfae.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gtqjeteqbx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtszspjhay.html

[R31] 局部变量
来源：http://hz.xziqi.cn/gtqbqpjaxv.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtxquyfemg.html

[R32] 参数个数校验
来源：http://hz.cdnleiting.top/gtdxxraqqu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gotoacloud.top/gtnmgfoaxl.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gtixknsrmn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtlvrmvkrh.html

[R34] 退出时清理
来源：http://hz.yongpay.top/gtrujicfpz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258888.top/gtjyqujhnh.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtznbdbbjv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtskkokttz.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtbcomnkof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.havefunace.top/gtftelykhm.html

[R37] 把输出赋给变量
来源：http://hz.jqgfzy.top/gtjdphrkls.html

files=$(ls -1)
来源：http://hz.nanxuanxn.top/gtjynedtqw.html

[R38] 管道串联
来源：http://hz.chenjidiqi.icu/gtiqfzddfh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtyrxwtewe.html

[R39] 重定向标准输出与错误
来源：http://hz.jianghu66.top/gtlkaefjvg.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtqgirtiiw.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtsljkmzeq.html

echo "log" >> out.log
来源：http://hz.cdnleiting.top/gtwxoeuhjo.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtbanqyaqr.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtjolrlrxj.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtbtpamwlz.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtinrecykm.html

[R43] 按名字查找文件
来源：http://hz.cdnleiting.top/gtaoukcxhh.html

find . -name "*.log" -type f
来源：http://hz.hysaishi.cn/gtofdjwydj.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtyxiypvdt.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtiouemkqq.html

[R45] 批量删除
来源：http://hz.haohaochexian.top/gtbyfjcmmx.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtlwqcffji.html

[R46] 递归替换文件内容
来源：http://hz.yongpay.top/gtnrutsmqr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtvezusrkq.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtyittvxnq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenlongwang.top/gtxepidfwb.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtuszxedlm.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtxjfnahij.html

[R49] awk 带条件
来源：http://hz.shzxlz.cn/gtapjkzlvh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtwzuachkb.html

[R50] awk 求和
来源：http://hz.hysaishi.cn/gtylnwtuif.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtklgyylkz.html

[R51] 排序去重取前几
来源：http://hz.yanxiufei.cn/gtihtforxh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtmrralcak.html

[R52] 统计行数
来源：http://hz.birdmap.top/gtffdxivtn.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtyykpises.html

[R53] 查看文件头与实时尾
来源：http://hz.hfpthk.cn/gtyyithdyp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtesfabaqp.html

[R54] 比较两个文件
来源：http://hz.zhengqikj.top/gtirjxvjec.html

diff a.txt b.txt
来源：http://hz.0kj1m.cn/gtxtmaatla.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtcumoimra.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtwszrkubq.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtcuugmied.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gthlahxshs.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtffqngobg.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtzsrqlwsc.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtloaogibu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fengsongda.top/gtbyaoyrlz.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtdlkoswzv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtwglokiee.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gtlmevwpjs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtygwwpcru.html

[R61] 磁盘占用
来源：http://hz.jiagoushi.top/gteiaxkusr.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtrkmmhhbc.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtuoccbamd.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtpxglcmce.html

[R63] 内存与进程
来源：http://hz.iojbl.cn/gtygazhsjj.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gtvqqcries.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtsozoxxhg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tanke756.top/gtvpqdrfzu.html

[R65] 查看端口占用
来源：http://hz.gaohongyu789.top/gtsjelzeux.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtuwwewezm.html

[R66] 定时任务
来源：http://hz.shanyushiyangkeji.top/gtbqsbbwis.html

crontab -e;  crontab -l
来源：http://hz.chenzaomai.com/gtinjojmtm.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtarhassqu.html


<!-- 参考信息 -->