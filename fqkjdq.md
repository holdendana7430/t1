代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xingfuxueyuan.xyz/gtecvgtwgz.html

[Q24] 去重
来源：http://hz.hfpthk.cn/gtmrbntgef.html

SELECT DISTINCT city FROM users;
来源：http://hz.haohaochexian.top/gtbsoajrps.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtzsaytehk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.smart0.xyz/gthyokfczt.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtzslfodwd.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtoiyzdsdl.html

[Q27] 条件计数
来源：http://hz.yj20258888.top/gtfiddzuoy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yongpay.top/gtechaxtcd.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtnmciaovk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sufxvd.cn/gtyojosdkd.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtmxhcfwrh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pycfn.com/gtuwjptzxc.html

[Q30] 分组统计
来源：http://hz.daria6918.cn/gtxrvsyqwq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtcxyuwawf.html

[Q31] 分组后过滤
来源：http://hz.jqgufenzy.top/gtdkrfcfrs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hfpthk.cn/gtgxnkbzvp.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtjyxgtnci.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtspomgdxh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtleewsonm.html

[Q33] 多列分组
来源：http://hz.yanxiufei.cn/gtsnezalym.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shzxlz.cn/gtzicgsrda.html

[Q34] 每组取第一条
来源：http://hz.daria6918.cn/gtukmglrih.html

SELECT * FROM (
来源：http://hz.ehwqpu.com/gtiximogau.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.52xcode.cn/gtsozuogtf.html

) t WHERE rn = 1;
来源：http://hz.xylfe.cn/gtevdpuvub.html

[Q35] 内连接
来源：http://hz.dianchejie.cn/gtwmdeazjz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtvrzkxlyb.html

[Q36] 左连接
来源：http://hz.gaohongyu789.top/gtxhlgmgph.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtitglgnbe.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gtxbqixrok.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gtbwjjxapo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.haohaochexian.top/gttphmaenw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.wangshuangyany.cn/gtkppponmt.html

[Q39] 自连接（查上下级）
来源：http://hz.jiagoushi.top/gtcbzhkdab.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gtgzqjedss.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj202588.top/gtycgemazb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgfzy.top/gtwvgqnixb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnqzz.top/gtgvbwmjym.html

[Q41] 多表连接
来源：http://hz.chenjidiqi.icu/gteqpjcjod.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuxming.cn/gtsijuagts.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gttvnayfvj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtbyubwxru.html

[Q42] 连接条件附加过滤
来源：http://hz.chenzaomai.com/gtprganjnl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtfrxsgori.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhixingplan.top/gtplmyvmti.html

[Q43] 标量子查询
来源：http://hz.yuanzhike.top/gtvyhcwjtt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtafudzhbn.html

[Q44] IN 子查询
来源：http://hz.pengpengdd.cyou/gtjpfuidlu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtkvxccwpq.html

[Q45] EXISTS 判断存在
来源：http://hz.0kj1m.cn/gtkvikgodj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtmgbtglfd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gtieyfuawr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtjjngsmdu.html

[Q47] 与平均值比较
来源：http://hz.316326.xyz/gtfasauphl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.svipenyu.cn/gtyuvygxai.html

[Q48] CTE 公用表表达式
来源：http://hz.vqdsnc.cn/gtpovagkgk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nanxuanxn.top/gttqqyubyr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtttbgxlvn.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtwlzetxbb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pycfn.com/gtqkkkpxno.html

[Q50] 批量更新
来源：http://hz.hywenlv.cn/gtzuxlotoh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xziqi.cn/gtzbjdpsba.html

[Q51] 用子查询更新
来源：http://hz.zycfv.cn/gtwjhqielj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhiwuduotai.top/gtttkugesa.html

[Q52] 删除指定行
来源：http://hz.havefunace.top/gtpvburxwr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.c1oappe.top/gtfoqikkcf.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtijikmjyo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtedbjpbra.html

[Q54] 清空表
来源：http://hz.zhaomingkeji.xyz/gturpxzwiy.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtpnwfxhvy.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtvasqdrew.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.bjfxy.top/gtcqtdzeyp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtzasoklqj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shangyingyoupin.top/gtuqwzyncf.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtmgzzahgg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.pengpengdd.cyou/gttkynqvyb.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtwmfljhsw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gotoacloud.top/gtbgzewxkl.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gtmolfkqnn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.c1oappe.top/gtbumdkzig.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangshuangyany.cn/gtglvgeowh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cashguo.top/gtomnubtvh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtugvlahwz.html

[Q61] 移动平均
来源：http://hz.daria6918.cn/gtgjssxfjw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangdashe.top/gtgdflzhtc.html

[Q62] 分组占比
来源：http://hz.hongshengwenyu.top/gtqkwtgyaj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtxduzambn.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtkhegeqna.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258.top/gtwvvqifrb.html

[Q64] 提交事务
来源：http://hz.jianghu66.top/gtgifoecmt.html

COMMIT;
来源：http://hz.chenjidiqi.icu/gtqlzoqdou.html

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtoctompav.html

ROLLBACK;
来源：http://hz.ivvv.top/gtvqjiedjd.html

[Q66] 行锁查询
来源：http://hz.wangshuangyany.cn/gtwhnuxnvw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.snrcjt.cn/gtdwcvmmwo.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtyroivujv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yangfankeji.com/gtqwiigcoy.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtcbgnjvvc.html

SAVEPOINT sp1;
来源：http://hz.jianghu66.top/gtofsyuano.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtgojimrjf.html

[Q69] 查看执行计划
来源：http://hz.pycfn.com/gtyuonxngm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cashguo.top/gtwlqrognn.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtvxcwcslo.html

ANALYZE TABLE users;
来源：http://hz.redwolf501.top/gtrqnowvvl.html

[Q71] 查看建表语句
来源：http://hz.xylfe.cn/gtwuwqrgcr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jlsjyb.cn/gtrefacpca.html

[Q72] 查看索引
来源：http://hz.chenjidiqi.icu/gtzyemxxaa.html

SHOW INDEX FROM users;
来源：http://hz.hysaishi.cn/gtwhuklnte.html

[Q73] 查看表状态
来源：http://hz.nwbrower.top/gtkokenfbo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinghuilouyu.cn/gtillfjmmo.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtvlxciljc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cashguo.top/gtisegbhen.html

[Q75] 日期格式化
来源：http://hz.shuidangran.top/gtvrriqtgt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cashguo.top/gtonfcxibm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtjauzovig.html

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtsvnirztr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ybcxt.top/gtmxsshroc.html

[Q77] 时间加减
来源：http://hz.hongshengwenyu.top/gtkbzmucsf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aibaodan.cn/gtuxllevyg.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gttvkbjpke.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gteisnqmdx.html

[Q79] 字符串拼接
来源：http://hz.jiagoushi.top/gttubctznx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hfpthk.cn/gtxileehve.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtavgqxiaq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtinxggiwu.html

[Q81] 字符串替换
来源：http://hz.pycfn.com/gtpgkoxzvl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhongyouzk.top/gtyxdagjjf.html

[Q82] 字符长度与字节长度
来源：http://hz.aibaodan.cn/gtyyeugwip.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ivvv.top/gtlbfpfirm.html

[Q83] 大小写转换
来源：http://hz.cqqwz.cn/gtnjmdxobm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.kuanghao11.cn/gtehpydrrl.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtokanrovp.html

SELECT TRIM(name) FROM users;
来源：http://hz.tianlin.xyz/gttbrqzaic.html

[Q85] 数值取整
来源：http://hz.jinqigufen.top/gtidfeeekx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gtxeshgyvz.html

[Q86] 读取 JSON 字段
来源：http://hz.52xcode.cn/gthpwtgmpm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgufenzy.top/gtuhuxkoub.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gtmnexubhw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhixingplan.top/gteeogumts.html

[Q88] 行转列（条件聚合）
来源：http://hz.snrcjt.cn/gtrcokwjbl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gthrxrlngm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtrqemcyyt.html

[Q89] 判断表是否存在
来源：http://hz.yj20258.top/gtfoeafpei.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.9152youxi.cn/gtinglzdrl.html

[Q90] 生成序号列
来源：http://hz.zhiwuduotai.top/gtcsfuoehu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tianlin.xyz/gtylzqvnpo.html

================================================================================
来源：http://hz.redwolf501.top/gthpiokprp.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtrdxmgozi.html

================================================================================
来源：http://hz.fengsongda.top/gtpqnecgqh.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtbtnoemxt.html

#!/usr/bin/env bash
来源：http://hz.zhoulong.xyz/gtghzbduzu.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtaqdzxwfa.html

[R02] 变量赋值与使用
来源：http://hz.jiagoushi.top/gtclpzpxvl.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtadsewzmv.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtaattabba.html

readonly PI=3.14
来源：http://hz.dashuyun.cn/gtytjicmuw.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtlgzqzzow.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gtnkjjklek.html

[R05] 参数默认值
来源：http://hz.andypj.xyz/gtwjnlogio.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtatvapxap.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtlhqywhja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydzc1.top/gtayzdnxqc.html

[R07] if 判断文件
来源：http://hz.meibo888.top/gtmqpzrvbp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxuanxn.top/gtycxdvbir.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtqikgyhff.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenjidiqi.icu/gtxudbnyrb.html

[R09] 字符串比较
来源：http://hz.c1oappe.top/gtyghxbomf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtnxnnyond.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gttiopjtvp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtmemxgrga.html

[R11] case 多分支
来源：http://hz.gogol.net.cn/gtsktudpqb.html

case "$1" in
来源：http://hz.cqqwz.cn/gtxvhdistp.html

start) echo "启动" ;;
来源：http://hz.xziqi.cn/gthjtnqqse.html

stop)  echo "停止" ;;
来源：http://hz.ybcxt.top/gthoqjziod.html

*)     echo "未知命令" ;;
来源：http://hz.cashguo.top/gtrbfzkagm.html

esac
来源：http://hz.yonumen.top/gtbtcrzhzv.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtmpotycxa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangtech.top/gtjjsygtfh.html

[R13] for 计数循环
来源：http://hz.52xcode.cn/gtcoednnvd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtbgblevvg.html

[R14] C 风格 for
来源：http://hz.yj20258.top/gtcouollzk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtgucmsrzq.html

[R15] while 逐行读文件
来源：http://hz.yuxming.cn/gtlhxnmqro.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxuanxn.top/gtkqbviotn.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtkwvysgqf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cucudq.cn/gtevyftetg.html

[R17] 数组定义与取值
来源：http://hz.yuxming.cn/gtbdwufrmj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtxyyqoeip.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtlinpddtq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenlongwang.top/gthcmmwznp.html

[R19] 数组长度
来源：http://hz.cdnleiting.top/gtzfbwmkrj.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtwposwowt.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtwczsbnjp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sxryk.cn/gtoknidycd.html

[R21] 字符串长度
来源：http://hz.sufxvd.cn/gtqjevrmnn.html

echo "${#s}"
来源：http://hz.ivvv.top/gtuhvsmfxx.html

[R22] 截取子串
来源：http://hz.redwolf501.top/gtwaryafpl.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtjlviigsr.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtmuqvhnyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtbbrtyvuo.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtamitfmhc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sweek.top/gtrhksheka.html

[R25] 去后缀 / 去前缀
来源：http://hz.ehwqpu.com/gtttzxhxez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtbbjittag.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtzyqybeqa.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtzrbzaayt.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtntptrcca.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtqtmaohuc.html

[R28] 浮点运算
来源：http://hz.yuxming.cn/gtogbmgbef.html

echo "scale=2; 10/3" | bc
来源：http://hz.shangyingyoupin.top/gthgmbupvg.html

[R29] 定义函数
来源：http://hz.zhijiandao.cn/gtvnryklak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtxycvhdgo.html

[R30] 函数返回状态码
来源：http://hz.yj202588.top/gtkwmiwyov.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtkklvaztw.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtwjwdraif.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtonsgqcfa.html

[R32] 参数个数校验
来源：http://hz.hongshengwenyu.top/gtcuuzszrf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.mhx1999.top/gtjqevizps.html

[R33] 捕获错误并提示行号
来源：http://hz.c1oappe.top/gtglfgnjhw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgfzy.top/gtbbcxjyqf.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtfmykyjzr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtziybcorj.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gtudldoadg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtzawofact.html

[R36] 并发执行多个任务
来源：http://hz.xingfuxueyuan.xyz/gtulfeyntg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sxryk.cn/gtxqjarypb.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtdarifelk.html

files=$(ls -1)
来源：http://hz.jinqigfzy.top/gtdcbpdchh.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gthatfeifi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtiimrvkbj.html

[R39] 重定向标准输出与错误
来源：http://hz.shzxlz.cn/gtrmttxyrk.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtguaativv.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtzwlmlytb.html

echo "log" >> out.log
来源：http://hz.nanxuanxn.top/gtthxxbwzr.html

[R41] 丢弃输出
来源：http://hz.cdnleiting.top/gtkmoirgep.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtqfrmlewp.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtzdukkqjk.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtgtauozea.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtvgkkhrfh.html

find . -name "*.log" -type f
来源：http://hz.fzhhl.top/gtqftgdbig.html

[R44] 按修改时间查找
来源：http://hz.yuanzhike.top/gtutrysuwp.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtcvzoqzam.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtudszxxpk.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtctyluipw.html

[R46] 递归替换文件内容
来源：http://hz.guowangkeji.top/gtkeqysiqg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gotoacloud.top/gtotlnongs.html

[R47] sed 单行替换
来源：http://hz.chenzaomai.com/gtrngjlqgp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hnqzz.top/gtwdpodrgi.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtmnzukrvz.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuanzhike.top/gtlvrkifkg.html

[R49] awk 带条件
来源：http://hz.yj202588.top/gtazuvrrks.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtsrhdwhei.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtilacczov.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xinyue.icu/gtdfmnzjyb.html

[R51] 排序去重取前几
来源：http://hz.yuanzhike.top/gtructmclp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ppjwa.cn/gtrqxjrmjd.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gtwlcluffc.html

wc -l a.txt
来源：http://hz.ivvv.top/gtjtkjftfj.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtquqdqgqr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtmsjyeirg.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtfeapemed.html

diff a.txt b.txt
来源：http://hz.nanxuanxn.top/gtdanqmyva.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gthdjbkskf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtcqnyfjez.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtebzqwlwa.html

scp file user@host:/path/
来源：http://hz.yj202588.top/gtotvsqbyf.html

[R57] 远程执行命令
来源：http://hz.zhaomingkeji.xyz/gtebfaulzf.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtfmzcuebk.html

[R58] 下载文件
来源：http://hz.iojbl.cn/gtpcbnmjlq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gthwqsbpkn.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtgapyzoed.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.haohaochexian.top/gtevdrollu.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtrhlzczhn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gtdvlcqhqc.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtvnnuamop.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtyymidesk.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gtakwanzfl.html

du -ah . | sort -rh | head -10
来源：http://hz.ppjwa.cn/gthuatyojt.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtjnvfydna.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtbumlsqsy.html

[R64] 结束进程
来源：http://hz.yueranfly.top/gtgkkfsxyc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtodbvqfsl.html

[R65] 查看端口占用
来源：http://hz.yongpay.top/gtoooputvy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtqxocvbyq.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtlsduogcj.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtpptjbeuh.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gtbahcxotu.html

openssl rand -hex 16
来源：http://hz.zhongyouzk.top/gtsuxummhi.html

[R68] 计算文件校验值
来源：http://hz.guannengcc.top/gtwpaicalz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daxiang520.top/gtvnvmdmug.html

[R69] 生成随机密码
来源：http://hz.316326.xyz/gtdfpuyepa.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gtdrmgpxvr.html

[R70] 时间戳与互转
来源：http://hz.zhongyouzk.top/gtrgeemdou.html

date +%s;  date -d @1700000000
来源：http://hz.c1oappe.top/gtbenezluw.html

[R71] 日期格式化
来源：http://hz.pycfn.com/gtsmnsliao.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtectsddss.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtvmxdghsf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtrpylfiui.html

[R73] 分割大日志
来源：http://hz.sxryk.cn/gtrjxlxlll.html


<!-- 参考信息 -->