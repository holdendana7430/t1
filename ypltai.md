代发 wailian999

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gthjaewwva.html

[Q16] 查询指定列
来源：http://hz.cdnleiting.top/gtolnahjda.html

SELECT id, name FROM users;
来源：http://hz.yongpay.top/gtjysghmxo.html

[Q17] 条件查询
来源：http://hz.gzhubu.top/gtqiqgyrpg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cqqwz.cn/gtmpatneaz.html

[Q18] 模糊匹配
来源：http://hz.hongshengwenyu.top/gttstzfpfx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gtzguznkbl.html

[Q19] 范围查询
来源：http://hz.yonumen.top/gthhkpyatt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fzhhl.top/gtuyahxrwk.html

[Q20] IN 列表
来源：http://hz.gaohongyu789.top/gtlqqbpkpm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yueranfly.top/gtiggfoabj.html

[Q21] 空值判断
来源：http://hz.yueranfly.top/gtaetxkxff.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhongyouzk.top/gtvdcybnvh.html

[Q22] 排序
来源：http://hz.yj20258.top/gtiieenhcb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.nanxinkj.top/gtagbdripd.html

[Q23] 分页
来源：http://hz.bjfxy.top/gtlifnhfon.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.mhx1999.top/gtdoynunac.html

[Q24] 去重
来源：http://hz.cdnleiting.top/gtjggwsfvc.html

SELECT DISTINCT city FROM users;
来源：http://hz.meibo888.top/gtauoctmgx.html

[Q25] 只取前 N 条
来源：http://hz.daxiang520.top/gteuuxvkql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhengqikj.top/gtwugrozpa.html

[Q26] 计数
来源：http://hz.ehwqpu.com/gteezoffrr.html

SELECT COUNT(*) FROM users;
来源：http://hz.ydjk.org.cn/gtajiflhtj.html

[Q27] 条件计数
来源：http://hz.cucudq.cn/gtmhjzdlah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhoulong.xyz/gtbjmgchoy.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtwcnamacn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hongshengwenyu.top/gtpebrkazb.html

[Q29] 最大最小值
来源：http://hz.nwbrower.top/gtggzrgbsx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cucudq.cn/gtwmholhqh.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtlgeoxbzu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtzsknfwhs.html

[Q31] 分组后过滤
来源：http://hz.ppjwa.cn/gtjzsihshi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtsdhcmkis.html

[Q32] 分组拼接字符串
来源：http://hz.wangdashe.top/gtgpllvolm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtzhjnzesr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gttdxacfzj.html

[Q33] 多列分组
来源：http://hz.nwbrower.top/gtcjfexeop.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtoyeswnsm.html

[Q34] 每组取第一条
来源：http://hz.zycfv.cn/gtqnhfzmah.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtdfrqtxle.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.snrcjt.cn/gtwuyydqrm.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtldhhfkhi.html

[Q35] 内连接
来源：http://hz.tanke756.top/gtqmslfbos.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtfxjfpclr.html

[Q36] 左连接
来源：http://hz.ivvv.top/gtapkcldtb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gthqohyajb.html

[Q37] 右连接
来源：http://hz.hnqzz.top/gtoenqluip.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtftcxesgj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtmydjnrph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangkeji.top/gtctyqvhlf.html

[Q39] 自连接（查上下级）
来源：http://hz.xingfuxueyuan.xyz/gtakgwcfxh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtrdqjecgx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtjyosekqo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tianlin.xyz/gtyxdldock.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhixingplan.top/gtxwyfxkvq.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gttdbgcbxo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtactyfjlh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtddfhphwi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuxming.cn/gtuychvzve.html

[Q42] 连接条件附加过滤
来源：http://hz.cucudq.cn/gtrpattxog.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jlsjyb.cn/gtdlhaqooz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj20258.top/gtrjqqebae.html

[Q43] 标量子查询
来源：http://hz.yj20258888.top/gtbspakpbn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtvrcnayzv.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtgicqpubg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gzhubu.top/gtkcskvubb.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258888.top/gtuckbyyda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtwpxvndwz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yueranfly.top/gtiehnfqha.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgfzy.top/gthktmflar.html

[Q47] 与平均值比较
来源：http://hz.daxiang520.top/gtfbrrmmar.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.bjfxy.top/gtrsscktoz.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gtvxrcnhyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtgnbdreei.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ppjwa.cn/gtiduijjrl.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtnqfzgcys.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xuetiantiany.cn/gtmjnjiwwy.html

[Q50] 批量更新
来源：http://hz.hnxiangtu.top/gtfbvsjeiq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hongshengwenyu.top/gtkztpugca.html

[Q51] 用子查询更新
来源：http://hz.xinyue.icu/gtgixipbpy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xuanzx.com/gtbppdacfn.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtyjryjste.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtkddnkfqj.html

[Q53] 按条件删除
来源：http://hz.c1oappe.top/gtexuzzjrm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gotoacloud.top/gtesfsmixe.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtlyiwqeuo.html

TRUNCATE TABLE logs;
来源：http://hz.cqqwz.cn/gtqmrrieft.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gtvxpiucqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtteovyakx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shangyingyoupin.top/gtqrnoqodh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigfzy.top/gtvbuuuejd.html

[Q57] 行号
来源：http://hz.daxiang520.top/gtnuofghth.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhoulong.xyz/gttzgiqsyj.html

[Q58] 累计求和
来源：http://hz.bjfxy.top/gtzwivrwvn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtiyohgwri.html

[Q59] 分组内累计
来源：http://hz.sweek.top/gtyffhuohq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.52xcode.cn/gtfbjoesis.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gtvifbdydi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gtzpcqptzt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yvedp.cn/gttjpettsu.html

[Q61] 移动平均
来源：http://hz.yj20258.top/gtmzsqhkdy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ydzc1.top/gtcxrbatwl.html

[Q62] 分组占比
来源：http://hz.quarkkingdee.top/gtoddvpmbd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtvqhdtxit.html

[Q63] 开启事务
来源：http://hz.yangfankeji.com/gtaxorrkcu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtkotbamoe.html

[Q64] 提交事务
来源：http://hz.yangfankeji.com/gthqsymatn.html

COMMIT;
来源：http://hz.iojbl.cn/gtxivftdyc.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtoqtyloak.html

ROLLBACK;
来源：http://hz.dianchejie.cn/gtecajqgjn.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtvgwpjtce.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.quarkkingdee.top/gtfxotzuhx.html

[Q67] 设置隔离级别
来源：http://hz.sysykeji.top/gtlqovemda.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtywpxgwdc.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtvrpbkwyy.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtjjxnrhpi.html

ROLLBACK TO sp1;
来源：http://hz.jlsjyb.cn/gtiaptyyjj.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtvcpzjhgz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuanzx.com/gtrxhjqzaq.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtsnpjljnh.html

ANALYZE TABLE users;
来源：http://hz.xuetiantiany.cn/gtziinkfta.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gtctpvxyeb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gthblmgkkw.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtmgyqjskk.html

SHOW INDEX FROM users;
来源：http://hz.9152youxi.cn/gtpxchyiqd.html

[Q73] 查看表状态
来源：http://hz.guannengcc.top/gtjcwdcqkk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gtjwpwrsno.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gteketgtlx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gzhubu.top/gtqsdbwdem.html

[Q75] 日期格式化
来源：http://hz.9152youxi.cn/gtwerntpdc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtebgziosz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtbfzxwfnr.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtrttubdcz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yvedp.cn/gtxantbwmq.html

[Q77] 时间加减
来源：http://hz.daxiang520.top/gtwhncricm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtpsmrwjpi.html

[Q78] 当前时间
来源：http://hz.ppjwa.cn/gtntltgils.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.52xcode.cn/gtmujkuier.html

[Q79] 字符串拼接
来源：http://hz.zdqjudy.top/gtukgawxul.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.mhx1999.top/gtfxamwkvs.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtzvrvaais.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtnripkodr.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtkqxdolww.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtubgpqvuh.html

[Q82] 字符长度与字节长度
来源：http://hz.smart0.xyz/gtcoqlzrze.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnxiangtu.top/gtdfqtjijf.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtzacmbsqz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtngptljpa.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtmvxadkrt.html

SELECT TRIM(name) FROM users;
来源：http://hz.daxiang520.top/gttgqlxwuo.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtjgurvvdm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtjzrfkypx.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtrbtrdjed.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.c1oappe.top/gtcfkfftuy.html

[Q87] JSON 字段做条件
来源：http://hz.guowangkeji.top/gtxestmaib.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtfnhftasc.html

[Q88] 行转列（条件聚合）
来源：http://hz.9152youxi.cn/gtjfttupsm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.smart0.xyz/gtdsemlips.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.quarkkingdee.top/gtlnvegfgh.html

[Q89] 判断表是否存在
来源：http://hz.hfpthk.cn/gtgtspxlis.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.birdmap.top/gtcemoccqy.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtiuxyxwjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtbzxhjqoc.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpyeosrfk.html

R. Bash 专题
来源：http://hz.yongpay.top/gtwzkfecmb.html

================================================================================
来源：http://hz.haohaochexian.top/gtohiwmumy.html

[R01] shebang 与严格模式
来源：http://hz.smart0.xyz/gtehwjygwq.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtytrugaoi.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtuueahrjx.html

[R02] 变量赋值与使用
来源：http://hz.dianchejie.cn/gtomjuynvv.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtiaauegwz.html

[R03] 只读变量
来源：http://hz.daria6918.cn/gtebearutr.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtykbypkow.html

[R04] 位置参数
来源：http://hz.chenlongwang.top/gtfkjnzbgx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jiagoushi.top/gtlrjcrgie.html

[R05] 参数默认值
来源：http://hz.316326.xyz/gtqitmhets.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtkvsuqelo.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gtcgvenimz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtxkhlsovb.html

[R07] if 判断文件
来源：http://hz.nanxuanxn.top/gtjpccjxlb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtczifbehw.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtqwpmmvsm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtxnvoxdqw.html

[R09] 字符串比较
来源：http://hz.aizwys.cn/gtnypomukz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtjzzlmixc.html

[R10] 正则匹配
来源：http://hz.ppjwa.cn/gtauglgoge.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydzc1.top/gtmwuohfud.html

[R11] case 多分支
来源：http://hz.andypj.xyz/gtgcqamtwo.html

case "$1" in
来源：http://hz.fengsongda.top/gtobfemxkq.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtvxahcqwz.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtarisifnm.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gtddtmquvr.html

esac
来源：http://hz.tianlin.xyz/gtpneunjra.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gtgjwsjjxn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xingfuxueyuan.xyz/gtoclljkmp.html

[R13] for 计数循环
来源：http://hz.tian-w.cn/gtelkmkcfn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtozplxzbe.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gthttcczlo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtseqmhgoe.html

[R15] while 逐行读文件
来源：http://hz.0kj1m.cn/gteoxdnwdx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guowangkeji.top/gtraszzewy.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtznzsgepw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtwkzdsdok.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtzlvsxluu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtxjqsdvpv.html

[R18] 遍历数组
来源：http://hz.quarkkingdee.top/gthcvgvnkp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtaupodirg.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gttxxchsop.html

echo "${#arr[@]}"
来源：http://hz.aibaodan.cn/gtmxnrstdj.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gtyhyyegqi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtvoshrsoc.html

[R21] 字符串长度
来源：http://hz.hfpthk.cn/gtgtukjxzm.html

echo "${#s}"
来源：http://hz.zycfv.cn/gtrezjeodk.html

[R22] 截取子串
来源：http://hz.gaohongyu789.top/gtggrlhlfw.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtecumxxuv.html

[R23] 字符串替换
来源：http://hz.cashguo.top/gtgmgfqdtz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gotoacloud.top/gttaxvoojr.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtujqquwgt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxuanxn.top/gtuvdedjhd.html

[R25] 去后缀 / 去前缀
来源：http://hz.hnqzz.top/gtqpqwydyh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinghuilouyu.cn/gtbxydbwik.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtteqnmuww.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtjeppolkr.html

[R27] 算术展开
来源：http://hz.ydjk.org.cn/gtdohhakxj.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtvxhtzlvd.html

[R28] 浮点运算
来源：http://hz.shanyushiyangkeji.top/gthiwemqwg.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gtphghmwpn.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtbvfbhlev.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aibaodan.cn/gtgibyyskk.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gtzpxnidok.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtjvbwhwch.html

[R31] 局部变量
来源：http://hz.tianlin.xyz/gtsaoopwgx.html

f() { local x=1; echo "$x"; }
来源：http://hz.cheryme.top/gtxprdtamv.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtmbszerrq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gtmqkiqbdl.html

[R33] 捕获错误并提示行号
来源：http://hz.xingfuxueyuan.xyz/gtcqvhebin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtwndtyljc.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gtjubeboss.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtqfzfvqmb.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtvujuaeqm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangtech.top/gtalfgabri.html

[R36] 并发执行多个任务
来源：http://hz.ywan-chungtsiang.top/gttftyqvpz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenzaomai.com/gtwyhpeunl.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gteaclsldn.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtcexympdz.html

[R38] 管道串联
来源：http://hz.chenjidiqi.icu/gtenyzmzvb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xylfe.cn/gtrsilqvik.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtrqlndecj.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtyysszmbt.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtsupurfkq.html

echo "log" >> out.log
来源：http://hz.zhoulong.xyz/gtfeqhgvmy.html

[R41] 丢弃输出
来源：http://hz.tian-w.cn/gtlkfyymox.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtgfnluiou.html

[R42] 输入重定向
来源：http://hz.aizwys.cn/gttfdidtwf.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtvwcivatg.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtbbrxbzxt.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gtdpnzhcsd.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtpcknwoyi.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtonbujsam.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gteunryhun.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtkvrpeqhd.html

[R46] 递归替换文件内容
来源：http://hz.yuanzhike.top/gtguasalqv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.316326.xyz/gtfnkubzsn.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtzcpkqwvi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtvllbcsfn.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtduxgslvz.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxinkj.top/gteviwwtkz.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtmrspswdo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtbowjhwcg.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtxejeprem.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhengqikj.top/gtzhkyefgh.html

[R51] 排序去重取前几
来源：http://hz.yj202588.top/gtqjbnmdwt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hysaishi.cn/gtgrxyskdp.html

[R52] 统计行数
来源：http://hz.shanyushiyangkeji.top/gtcgemaxxn.html

wc -l a.txt
来源：http://hz.316326.xyz/gtobqwbklr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtjnhmhmig.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gtivbiiatu.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtluschbjo.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gttgrbpcks.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtrlmgjsms.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtekeueiyj.html

[R56] 远程拷贝
来源：http://hz.guannengcc.top/gtjfnuopdv.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gtxmjhownb.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gtlcrzvxuo.html

ssh user@host 'uptime'
来源：http://hz.chenlongwang.top/gtymegeoub.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gtaooojukv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtaszxvpyh.html

[R59] 发 POST JSON
来源：http://hz.birdmap.top/gttfcoasjp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtqtzvrwdv.html

[R60] 只看 HTTP 状态码
来源：http://hz.zdqjudy.top/gtsohtyyge.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yuanzhike.top/gtcdhkstxp.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtvqjoxpoq.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtkiwfgpzj.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gthczwdxao.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangkeji.top/gtjtzfzbus.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtykxjvdwz.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gthbbkdgif.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtvmvwbhjq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cucudq.cn/gtwneoxyky.html

[R65] 查看端口占用
来源：http://hz.tanke756.top/gtaojxfczd.html


<!-- 参考信息 -->