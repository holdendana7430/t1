代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtaxzfxgnu.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gttwqamxle.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cucudq.cn/gtgfaniekw.html

[Q19] 范围查询
来源：http://hz.chenlongwang.top/gtvwbtuydd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yvedp.cn/gtxqpjfvqf.html

[Q20] IN 列表
来源：http://hz.zhoulong.xyz/gtrykavbyg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.haohaochexian.top/gtireitiei.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtmkhgadxb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtojjbibzr.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtvdhwrnfl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zycfv.cn/gtkuvqzuzb.html

[Q23] 分页
来源：http://hz.jqgufenzy.top/gtzanczhct.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daxiang520.top/gtcaitzybz.html

[Q24] 去重
来源：http://hz.iojbl.cn/gteudilrnh.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhixingplan.top/gtuahgdetl.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtdkpapwic.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinghuilouyu.cn/gtrywoojaf.html

[Q26] 计数
来源：http://hz.aizwys.cn/gtgvogqdvc.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258888.top/gtjwjccuyf.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtplyozgka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yueranfly.top/gtatturpxu.html

[Q28] 求和与平均
来源：http://hz.0kj1m.cn/gtdbmbkdgw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fengsongda.top/gtzdxmyffo.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtvhcxfwlc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinghuilouyu.cn/gttbeffblg.html

[Q30] 分组统计
来源：http://hz.yj20258888.top/gticepuwer.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtpwxkhemh.html

[Q31] 分组后过滤
来源：http://hz.shuidangran.top/gtllgopwge.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtydrkxerm.html

[Q32] 分组拼接字符串
来源：http://hz.c1oappe.top/gttindntit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtbwnoeewq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.tanke756.top/gtnsfbwbeh.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtarbozkjy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.fengsongda.top/gtwlacscck.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtcssmenxs.html

SELECT * FROM (
来源：http://hz.chenzaomai.com/gttkpfsjqm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.iojbl.cn/gtlpvnlxft.html

) t WHERE rn = 1;
来源：http://hz.svipenyu.cn/gtpiqvixif.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtwjrirror.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtwydgdfxu.html

[Q36] 左连接
来源：http://hz.cucudq.cn/gtjjosrksp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtrogglngv.html

[Q37] 右连接
来源：http://hz.pycfn.com/gtkvdchrtv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aizwys.cn/gthpbezwoe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258.top/gtivcytyib.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangkeji.top/gtqxgtixii.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtigrxgjhi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ppjwa.cn/gtvryekqsb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ppjwa.cn/gtddofzrsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tianlin.xyz/gtajwcgmju.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtwtjznqnh.html

[Q41] 多表连接
来源：http://hz.zhixingplan.top/gtlafxneyc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtmfzxbacl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.andypj.xyz/gttemoscke.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gthggfryms.html

[Q42] 连接条件附加过滤
来源：http://hz.zhaomingkeji.xyz/gtwjeilspy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shangyingyoupin.top/gtyvdzkgqy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gtpwlewuoj.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtlfxmdwmo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.c1oappe.top/gtnggbasno.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtuptseeci.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cdnleiting.top/gtbsxiurbh.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtjjsugvub.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtqmfiulxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuanzhike.top/gtbnkpylbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtgcmozsln.html

[Q47] 与平均值比较
来源：http://hz.jinqigufen.top/gtenapwcjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gthdjcvcbf.html

[Q48] CTE 公用表表达式
来源：http://hz.jinyuanbaomall.cn/gtajcwxphx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtywvlmvmg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtcsbsapia.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtmeybzzdz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ehwqpu.com/gtszedprny.html

[Q50] 批量更新
来源：http://hz.yanxiufei.cn/gtzhmlmgrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtjaebbwzl.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtfwhteamr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtzsaukrll.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gtgnypgnfc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtawlrbtie.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtxzlmrwwe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtfxetqouy.html

[Q54] 清空表
来源：http://hz.sweek.top/gtgafnhgmk.html

TRUNCATE TABLE logs;
来源：http://hz.birdmap.top/gtssmnossw.html

[Q55] 排名（并列占位）
来源：http://hz.hongshengwenyu.top/gtsrmegamt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtdgppskeq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigufen.top/gtysagetld.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtegaibbzv.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtgsknohdw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtrobkudne.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtbjlxvudx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gttxgyxeil.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtolgqsrig.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtvsdgejrj.html

[Q60] 取上一行 / 下一行
来源：http://hz.yangfankeji.com/gtbpttxxcp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gttetlvluy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhongyouzk.top/gtfpvokcsg.html

[Q61] 移动平均
来源：http://hz.aibaodan.cn/gtmnftylbs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ydzc1.top/gtbfilhyuy.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gtyafeaaqy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtbycnowkl.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtaijmpkqh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tianlin.xyz/gtchpjihtx.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtsdxlgcox.html

COMMIT;
来源：http://hz.jinghuilouyu.cn/gtuslmtddz.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtmvxljbps.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtxeommqtb.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtwupeqpry.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtjdzyyiqe.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtftmnsadj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtrhgeanno.html

[Q68] 保存点
来源：http://hz.snrcjt.cn/gtpiywlszb.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtsrkyjyzx.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtljjhiwbj.html

[Q69] 查看执行计划
来源：http://hz.sufxvd.cn/gteilgdzrk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtcemzcnhh.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtnwicpegn.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtfahmupbb.html

[Q71] 查看建表语句
来源：http://hz.shzxlz.cn/gtgmqywmfo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.0kj1m.cn/gtotvbqlhx.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtyswwcbof.html

SHOW INDEX FROM users;
来源：http://hz.guannengcc.top/gtddukdtem.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtyfhpqeoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gtwgyrzxze.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtddbmwsta.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gteyfslnue.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtecevgcfe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aibaodan.cn/gtrroqthmi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtfireolca.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtoxnbylvd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hongshengwenyu.top/gtrnvviqsd.html

[Q77] 时间加减
来源：http://hz.redwolf501.top/gtbithfuna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gogol.net.cn/gtujixhtxv.html

[Q78] 当前时间
来源：http://hz.jinqigufen.top/gtfjcdnxnr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhongyouzk.top/gtlowzyajv.html

[Q79] 字符串拼接
来源：http://hz.zhoulong.xyz/gtinfbwztr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtglmwmdkx.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gtrlgleqai.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.andypj.xyz/gtajlrkoap.html

[Q81] 字符串替换
来源：http://hz.yanxiufei.cn/gtbpxksusz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xuanzx.com/gttkplmnyl.html

[Q82] 字符长度与字节长度
来源：http://hz.snrcjt.cn/gtvoytabsp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ybcxt.top/gtdxuxxdtn.html

[Q83] 大小写转换
来源：http://hz.hongshengwenyu.top/gtekudjzew.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtgybzyaff.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gtxauttxle.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtcisviuec.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtcuajzdfl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gtjtmsaces.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtgwyktahx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.smart0.xyz/gtwhluozlu.html

[Q87] JSON 字段做条件
来源：http://hz.hysaishi.cn/gtreswiwlx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yueranfly.top/gtfddyoqfp.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtrpouxaqa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhaomingkeji.xyz/gtwuikupbz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xinyue.icu/gtardamioo.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtnedrhers.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.c1oappe.top/gtuyucrnmv.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtwpuhhkye.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtiburmase.html

================================================================================
来源：http://hz.jqgfzy.top/gtsuamhmrp.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtbirdszwj.html

================================================================================
来源：http://hz.fzhhl.top/gtiklzevvl.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtmdxagdnp.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtdzlqwxjc.html

set -euo pipefail
来源：http://hz.gotoacloud.top/gtssgwtndv.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gtxibnryve.html

name="Tom"; echo "$name"
来源：http://hz.jlsjyb.cn/gtgptqufln.html

[R03] 只读变量
来源：http://hz.wangshuangyany.cn/gtzobnnuja.html

readonly PI=3.14
来源：http://hz.aibaodan.cn/gtuwatvhvy.html

[R04] 位置参数
来源：http://hz.nwbrower.top/gtdilzhjhv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.smart0.xyz/gtuucxihyq.html

[R05] 参数默认值
来源：http://hz.xziqi.cn/gtlmitrabg.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtjffyjarn.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtpshpbwgp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xziqi.cn/gtcziymwll.html

[R07] if 判断文件
来源：http://hz.meibo888.top/gtapeohbsd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtfmmzwjvw.html

[R08] 数值比较
来源：http://hz.gotoacloud.top/gtteuqfndv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtqxzkyxmn.html

[R09] 字符串比较
来源：http://hz.jqgfzy.top/gtqmjkydwp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.guannengcc.top/gtlbjzhqeq.html

[R10] 正则匹配
来源：http://hz.kuanghao11.cn/gtyonnydwz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hywenlv.cn/gtfsdesjgs.html

[R11] case 多分支
来源：http://hz.dianchejie.cn/gtonggogln.html

case "$1" in
来源：http://hz.tian-w.cn/gtmkcjohfi.html

start) echo "启动" ;;
来源：http://hz.sxryk.cn/gtfazypssd.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtiyphavgt.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gteewxvxfx.html

esac
来源：http://hz.xinyue.icu/gtsutdeeoj.html

[R12] for 遍历文件
来源：http://hz.nanxuanxn.top/gtiegqrltw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydzc1.top/gtipfcofvd.html

[R13] for 计数循环
来源：http://hz.jyoumei.cn/gtrrhzioah.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.daxiang520.top/gtpbghdfnz.html

[R14] C 风格 for
来源：http://hz.hnxiangtu.top/gtewtbgoln.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gtwsalodvl.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtlplruuac.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.redwolf501.top/gtpafbgjql.html

[R16] until 等待条件
来源：http://hz.zhoulong.xyz/gtmrztypzn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtxnjhiutj.html

[R17] 数组定义与取值
来源：http://hz.jiagoushi.top/gtsohwvfhx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tianlin.xyz/gtbdtgaifr.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtigmfilat.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cashguo.top/gtoymdwhyx.html

[R19] 数组长度
来源：http://hz.havefunace.top/gttpqgnnxu.html

echo "${#arr[@]}"
来源：http://hz.xylfe.cn/gtvudwzemg.html

[R20] 关联数组（字典）
来源：http://hz.0kj1m.cn/gtnbsvvcps.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.smart0.xyz/gtxygpcohf.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtedyoslvn.html

echo "${#s}"
来源：http://hz.sweek.top/gtubqkqojg.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gttljbmpqs.html

echo "${s:0:5}"
来源：http://hz.meibo888.top/gtalogveeq.html

[R23] 字符串替换
来源：http://hz.ydjk.org.cn/gtkylnnqgp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigufen.top/gtbpbleawy.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gtgifjaktu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangkeji.top/gtytewxteh.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenlongwang.top/gtdshkhfjp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtogzpifhg.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtzlrcnvla.html

now=$(date +%F); echo "$now"
来源：http://hz.mhx1999.top/gtmzwclrdf.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtibojnytk.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtxpudirop.html

[R28] 浮点运算
来源：http://hz.yonumen.top/gtjpxwgdqf.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtuonpvixh.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtixzugqji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtwapsblgq.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gtvgowruqz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinghuilouyu.cn/gtubdwzumr.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtkhifavkh.html

f() { local x=1; echo "$x"; }
来源：http://hz.jyoumei.cn/gtmiynfryv.html

[R32] 参数个数校验
来源：http://hz.fengsongda.top/gtgtpmtytd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gttvdrcgjg.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258.top/gtxkuayynf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhiwuduotai.top/gtxgcyfhgu.html

[R34] 退出时清理
来源：http://hz.zhiwuduotai.top/gtscimvlur.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtigaiceie.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtokwfjhkf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtestodoji.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtyxyzpqwp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.birdmap.top/gtiiauxnvc.html

[R37] 把输出赋给变量
来源：http://hz.pengpengdd.cyou/gtkrptsztq.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtnibomdek.html

[R38] 管道串联
来源：http://hz.yueranfly.top/gtlpbfpdwh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtuibwensn.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtiriedcqh.html

cmd > out.log 2>&1
来源：http://hz.ywan-chungtsiang.top/gtrcnwzhzx.html

[R40] 追加写日志
来源：http://hz.ybcxt.top/gtpmazwbeo.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtldopbqib.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtpdnpclph.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtkpyeayhg.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtoegpftvy.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtfvalkofz.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtnytanvei.html

find . -name "*.log" -type f
来源：http://hz.sufxvd.cn/gtmzflctbs.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gtuzylnnkg.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gtwyjimykh.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtewothojr.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtejeufdja.html

[R46] 递归替换文件内容
来源：http://hz.svipenyu.cn/gtorpuibxp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtwhrnhejg.html

[R47] sed 单行替换
来源：http://hz.jinqigufen.top/gtorjvpkxy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jlsjyb.cn/gtbyvpveqy.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtzywqtstx.html

awk '{print $1, $3}' a.txt
来源：http://hz.quarkkingdee.top/gtyifprlsq.html

[R49] awk 带条件
来源：http://hz.zhengqikj.top/gtzbainijl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cashguo.top/gtarurkndk.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtxcerzczn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtnupzdgef.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangkeji.top/gtnjafagsd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.birdmap.top/gtcgffzqyf.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtlegqrdzj.html

wc -l a.txt
来源：http://hz.sweek.top/gteekwavbs.html

[R53] 查看文件头与实时尾
来源：http://hz.gotoacloud.top/gtdvyncyoe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtvrdriuqp.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gteoydyngm.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtbfelulbb.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtoueintmw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gthvfkstel.html

[R56] 远程拷贝
来源：http://hz.svipenyu.cn/gtvdbfemgv.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtordtgmwf.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtbmdduscx.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gtdvfruvgf.html

[R58] 下载文件
来源：http://hz.ybcxt.top/gtzfpijxdb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgufenzy.top/gtfwtjxxyt.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtnzhcpjmg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtskvdrlqz.html

[R60] 只看 HTTP 状态码
来源：http://hz.316326.xyz/gtejxnvhbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hywenlv.cn/gtlvjqbhni.html

[R61] 磁盘占用
来源：http://hz.zhoulong.xyz/gtoyomvqdj.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtkdglyqzg.html

[R62] 找最占空间的文件
来源：http://hz.iojbl.cn/gtopuejtrr.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtqexkkoav.html

[R63] 内存与进程
来源：http://hz.quarkkingdee.top/gtlnhqvgov.html

free -h;  ps aux | grep nginx
来源：http://hz.jinghuilouyu.cn/gtdolgqnrl.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtcddmtmmm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtlboxyhoo.html

[R65] 查看端口占用
来源：http://hz.zhoulong.xyz/gtxopympru.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtbtoxilsh.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gteuajkohg.html

crontab -e;  crontab -l
来源：http://hz.xinyue.icu/gtxttbsdtw.html

[R67] 生成随机十六进制串
来源：http://hz.zhongyouzk.top/gtybhklmlh.html


<!-- 参考信息 -->