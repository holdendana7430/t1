代发 wailian999

SELECT * FROM users;
来源：http://hz.jqgufenzy.top/gtfemnzhog.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtswrymtnn.html

SELECT id, name FROM users;
来源：http://hz.zdqjudy.top/gtquecnceq.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gtwnjjcpra.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.snrcjt.cn/gteuwtrazx.html

[Q18] 模糊匹配
来源：http://hz.birdmap.top/gtwjgdkymb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xziqi.cn/gtpbfluaze.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gtujaahxqe.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtpitismzz.html

[Q20] IN 列表
来源：http://hz.aizwys.cn/gtqdertdlj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yuxming.cn/gtbqdnmnjh.html

[Q21] 空值判断
来源：http://hz.yj20258.top/gtwcunvoxu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangkeji.top/gtqpiysjeu.html

[Q22] 排序
来源：http://hz.hnxiangtu.top/gtryfbcymk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ywan-chungtsiang.top/gtxjssbvzn.html

[Q23] 分页
来源：http://hz.jyoumei.cn/gtwgpmcvqx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daria6918.cn/gttleyogtl.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gthxzctewl.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtlctkrbvz.html

[Q25] 只取前 N 条
来源：http://hz.yongpay.top/gtclsrwrte.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nwbrower.top/gtybvzccwj.html

[Q26] 计数
来源：http://hz.pycfn.com/gtlmoxqtvq.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhoulong.xyz/gtjvjcmvup.html

[Q27] 条件计数
来源：http://hz.gogol.net.cn/gtxfuzsuwo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gtvdjlomus.html

[Q28] 求和与平均
来源：http://hz.jqgfzy.top/gtxopuslhu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daxiang520.top/gtnkscoila.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtisqpcigg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtqdvwleeo.html

[Q30] 分组统计
来源：http://hz.gogol.net.cn/gtuhozhcnd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtpuwoxqqs.html

[Q31] 分组后过滤
来源：http://hz.yvedp.cn/gtjbuuuquj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenzaomai.com/gtrkhciokf.html

[Q32] 分组拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtlmbwuqvb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtjdynlpqn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxuanxn.top/gtaipstxyk.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtusbkbanl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xziqi.cn/gtycgqaeca.html

[Q34] 每组取第一条
来源：http://hz.sysykeji.top/gtbzxhavqj.html

SELECT * FROM (
来源：http://hz.tianlin.xyz/gtveowkbqk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenzaomai.com/gteoomlvax.html

) t WHERE rn = 1;
来源：http://hz.jinyuanbaomall.cn/gtoyvtoapj.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtmxnwqblr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtdkyopsgv.html

[Q36] 左连接
来源：http://hz.52xcode.cn/gtzabneysr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.316326.xyz/gtmdmygyuq.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtbkukulyq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangdashe.top/gtynuqdgfo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgufenzy.top/gtfpniybov.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258888.top/gtqzfalxfw.html

[Q39] 自连接（查上下级）
来源：http://hz.jlsjyb.cn/gtnqvqvtqg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtkwmvxgsn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtqdjvyudq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258.top/gtherznxmi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.snrcjt.cn/gtkqsmpozh.html

[Q41] 多表连接
来源：http://hz.ywan-chungtsiang.top/gtbjmhjzml.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtsoaacjwy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtykbyrczl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtusmoopel.html

[Q42] 连接条件附加过滤
来源：http://hz.xuetiantiany.cn/gtvtuuulmg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hysaishi.cn/gtilchxovl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtxijrfzvt.html

[Q43] 标量子查询
来源：http://hz.hysaishi.cn/gtqubcdzqe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gttuzbpttm.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtegvoxore.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtqxhqhvpa.html

[Q45] EXISTS 判断存在
来源：http://hz.hongshengwenyu.top/gtwxpozggt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtskcgilrz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.guannengcc.top/gtdborhgui.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtsdqxdujl.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtolwptjji.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.0kj1m.cn/gtujdenygw.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gtolrlfqqq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ywan-chungtsiang.top/gthzxyluoq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gotoacloud.top/gtodfmovka.html

[Q49] 更新单行
来源：http://hz.hysaishi.cn/gtnkyxlypk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.svipenyu.cn/gtpqdedncl.html

[Q50] 批量更新
来源：http://hz.zhixingplan.top/gtnyqbcidr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pycfn.com/gtgfacvfzh.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gttexovgvw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yanxiufei.cn/gtkstxzglq.html

[Q52] 删除指定行
来源：http://hz.xziqi.cn/gtsawhcvcv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenjidiqi.icu/gtujdvgoos.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gthjxlcnty.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yuanzhike.top/gtujdqdiif.html

[Q54] 清空表
来源：http://hz.sysykeji.top/gtowcqvcty.html

TRUNCATE TABLE logs;
来源：http://hz.hnxiangtu.top/gtqxzgtpxg.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gttiupjrjt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gzhubu.top/gtcphklowp.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigufen.top/gtvbaifwkn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gtwbdcuwxr.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtixkjtfim.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.tianlin.xyz/gtanmjddqd.html

[Q58] 累计求和
来源：http://hz.hammf.cn/gtdxrufgyx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.svipenyu.cn/gtkfrsjafc.html

[Q59] 分组内累计
来源：http://hz.zhijiandao.cn/gtgzdacvku.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tianlin.xyz/gtfuhktiiy.html

[Q60] 取上一行 / 下一行
来源：http://hz.dianchejie.cn/gtbyhalxvo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtbtobtqpv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtnetyorrq.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtjhqyajgm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtmxsrnrsh.html

[Q62] 分组占比
来源：http://hz.aibaodan.cn/gtvuudozit.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gttsgijccr.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gtayanczkh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtzvtwbzop.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtblrfgxvb.html

COMMIT;
来源：http://hz.havefunace.top/gteqbpxgff.html

[Q65] 回滚事务
来源：http://hz.wangshuangyany.cn/gtktxrfivq.html

ROLLBACK;
来源：http://hz.nwbrower.top/gtbmcowyks.html

[Q66] 行锁查询
来源：http://hz.smart0.xyz/gtbdubvlrw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.mhx1999.top/gtdaztrwhj.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtukrzdlfw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydzc1.top/gtqnzqjtst.html

[Q68] 保存点
来源：http://hz.meibo888.top/gtvvjojcfd.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtahhgznso.html

ROLLBACK TO sp1;
来源：http://hz.zhoulong.xyz/gtrkzgbtli.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtglfevsko.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtrhudtmsm.html

[Q70] 更新统计信息
来源：http://hz.xuetiantiany.cn/gtygbgockc.html

ANALYZE TABLE users;
来源：http://hz.birdmap.top/gtrfjptupk.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtncwzbadd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gthycwihuz.html

[Q72] 查看索引
来源：http://hz.xuanzx.com/gttrsuoqtf.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtmjzslqfp.html

[Q73] 查看表状态
来源：http://hz.gaohongyu789.top/gtdpekzopy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zycfv.cn/gtlwpltayd.html

[Q74] 强制使用索引
来源：http://hz.aibaodan.cn/gtyfxghnmr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtjqmcctvu.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtriawjlbq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtuubcszxh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gtkgnqewsy.html

[Q76] 按天统计
来源：http://hz.sweek.top/gtwhuzezfn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.vqdsnc.cn/gtxofjogzd.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtvbzdexjb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shzxlz.cn/gtlmtaswwz.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gttxsvlymy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtmywykste.html

[Q79] 字符串拼接
来源：http://hz.shangyingyoupin.top/gtqlgqbspo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.c1oappe.top/gtjsanrlwe.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtnvbovzkk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtbqfvyter.html

[Q81] 字符串替换
来源：http://hz.xinyue.icu/gtltsyuyvv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gzhubu.top/gtudmmujbo.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gtczvdarer.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cdnleiting.top/gtjrqbfdlz.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtcvzpvayu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtpuaypeox.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gteibbhxza.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydjk.org.cn/gtaxkvitdx.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtamkjlgpq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gthiadepax.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtznvbichn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tianlin.xyz/gtmsruggbb.html

[Q87] JSON 字段做条件
来源：http://hz.yanxiufei.cn/gtdndrlhkx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhixingplan.top/gtvroywcdw.html

[Q88] 行转列（条件聚合）
来源：http://hz.haohaochexian.top/gtyfehuadl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yongpay.top/gtinoepbhu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guannengcc.top/gtcvnyrmwn.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtmwxactaj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gttmwfrrgi.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtxgngqtsq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cashguo.top/gtglfniifs.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqagqmoui.html

R. Bash 专题
来源：http://hz.zhiwuduotai.top/gtbeegqkdp.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpxeqcnhs.html

[R01] shebang 与严格模式
来源：http://hz.yuxming.cn/gtxqhbgnmr.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtzwbmxijg.html

set -euo pipefail
来源：http://hz.ivvv.top/gtrvqqpobf.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtfeloitma.html

name="Tom"; echo "$name"
来源：http://hz.iojbl.cn/gtdhzgvfnj.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gterymqcxp.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtjhehlgee.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gtkmfuspbu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gthbiksxci.html

[R05] 参数默认值
来源：http://hz.fzhhl.top/gtbctlahdh.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtfmylsuxp.html

[R06] 判断命令是否存在
来源：http://hz.tianlin.xyz/gtfyhwderg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtrfrrtzif.html

[R07] if 判断文件
来源：http://hz.316326.xyz/gtgjsfcfyz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gtfajwddde.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtoiuadjdg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydzc1.top/gtgrlzydfc.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gtlczpmyzz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtndrwydzs.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtcydcclue.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtqfrhhbus.html

[R11] case 多分支
来源：http://hz.zhixingplan.top/gtyheajejb.html

case "$1" in
来源：http://hz.chenzaomai.com/gtsmdtjpwk.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtegggntns.html

stop)  echo "停止" ;;
来源：http://hz.jqgfzy.top/gtksjsbivt.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtfkpspadb.html

esac
来源：http://hz.yanxiufei.cn/gtkhpdfmef.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtdbuybqws.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gtdpnaulin.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtyhidgawg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.mhx1999.top/gtdjdiutbx.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtsorzwcqy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtubnrebcr.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtsgmdubyg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtfxteebaq.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtxsskjvuv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtpamzqvet.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtzqvrwkkx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtgzyphvjl.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtyqqphnaz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pengpengdd.cyou/gtuwwpqodi.html

[R19] 数组长度
来源：http://hz.yueranfly.top/gtwizgwxht.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gtudoirkgr.html

[R20] 关联数组（字典）
来源：http://hz.jinghuilouyu.cn/gtkcymnvea.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtqjmiuakj.html

[R21] 字符串长度
来源：http://hz.jiagoushi.top/gtvjbeszvg.html

echo "${#s}"
来源：http://hz.yangfankeji.com/gtszwkkout.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtvpfaiind.html

echo "${s:0:5}"
来源：http://hz.hnqzz.top/gtczrvxiny.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gtxilmfykv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.andypj.xyz/gtydruufzh.html

[R24] 大小写转换
来源：http://hz.guowangkeji.top/gttbehadjm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.mhx1999.top/gtuozxjrjp.html

[R25] 去后缀 / 去前缀
来源：http://hz.smart0.xyz/gtwtrnoses.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gtqfqwhwax.html

[R26] 命令替换
来源：http://hz.tanke756.top/gtmbekqodf.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtuqsqqwvg.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gttpfnlhiq.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtijaeyxga.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtcpcmlwid.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtawnwxqur.html

[R29] 定义函数
来源：http://hz.hfpthk.cn/gtpirokfls.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dashuyun.cn/gtlfzsjqpq.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gtkadmfwna.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtzvaqzfvi.html

[R31] 局部变量
来源：http://hz.bjfxy.top/gtrhcwumrb.html

f() { local x=1; echo "$x"; }
来源：http://hz.iojbl.cn/gtluwmpgwx.html

[R32] 参数个数校验
来源：http://hz.nwbrower.top/gtinzzuppu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gtqknwzmor.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtnirkfaxh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtqbkfoibg.html

[R34] 退出时清理
来源：http://hz.cdnleiting.top/gtulokbdpk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtpltzsxqr.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtqpwvejnq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtybegbjvk.html

[R36] 并发执行多个任务
来源：http://hz.chenjidiqi.icu/gtzggeevnm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtuyckiluw.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtyzstdsbk.html

files=$(ls -1)
来源：http://hz.daxiang520.top/gtuoqffeqj.html

[R38] 管道串联
来源：http://hz.ywan-chungtsiang.top/gtpxsclqvd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtvxjnqtvy.html

[R39] 重定向标准输出与错误
来源：http://hz.0kj1m.cn/gtdsqwvvjz.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtrgzlyipv.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtqjlyajmf.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gtgwupalql.html

[R41] 丢弃输出
来源：http://hz.tianlin.xyz/gtypcomwum.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtytqfzady.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtjrcqfguc.html

wc -l < a.txt
来源：http://hz.yonumen.top/gtxosteouk.html

[R43] 按名字查找文件
来源：http://hz.yj20258.top/gtsijqcnvo.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gteerwjbbn.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtkfwdkrrn.html

find . -mtime -7 -type f
来源：http://hz.hammf.cn/gtiryvznbh.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtsvehebmv.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtbvmuyfks.html

[R46] 递归替换文件内容
来源：http://hz.snrcjt.cn/gtnewrereb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtophoflef.html

[R47] sed 单行替换
来源：http://hz.dianchejie.cn/gtvyaxevwh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shzxlz.cn/gticignchs.html

[R48] awk 取指定列
来源：http://hz.yonumen.top/gtxijuvmag.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangtech.top/gtsmjkzwre.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtpkbztgex.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtklupijye.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtdpykhbxm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtrtssunob.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gtbuemiqhp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuanzhike.top/gthoiiztwg.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gtraceirlv.html

wc -l a.txt
来源：http://hz.jlsjyb.cn/gtdwdmaaue.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtzhnvobmu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.redwolf501.top/gtuqkngcaz.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtqzidqcvo.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gthtfnnmhj.html

[R55] 压缩与解压
来源：http://hz.tian-w.cn/gtmfzmhdlb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtcmgquwrn.html

[R56] 远程拷贝
来源：http://hz.shangyingyoupin.top/gtwgqakdyz.html

scp file user@host:/path/
来源：http://hz.dianchejie.cn/gtqsqdyigm.html

[R57] 远程执行命令
来源：http://hz.zhengqikj.top/gtmlskxtnf.html

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtaterhrni.html

[R58] 下载文件
来源：http://hz.ydjk.org.cn/gthqqrteyi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtfmefjczz.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtssfyfjbq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtloqktcft.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtrxhaldtq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daria6918.cn/gthemvuajv.html

[R61] 磁盘占用
来源：http://hz.daria6918.cn/gtqxjvgack.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtumvsbukl.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtfggyzjzf.html

du -ah . | sort -rh | head -10
来源：http://hz.hywenlv.cn/gtmuvagiuh.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtoxegmvgt.html

free -h;  ps aux | grep nginx
来源：http://hz.birdmap.top/gtzzpsebpy.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtjkuljmye.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fengsongda.top/gtxbylavak.html

[R65] 查看端口占用
来源：http://hz.zhengqikj.top/gthbtrrdet.html


<!-- 参考信息 -->