代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gotoacloud.top/gtkbhezgrr.html

[Q24] 去重
来源：http://hz.yanxiufei.cn/gtcbdcxhrg.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhoulong.xyz/gtsjunqugr.html

[Q25] 只取前 N 条
来源：http://hz.sxryk.cn/gtyqttzfyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtmwkhsing.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtnihejsgk.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtnqkthfqp.html

[Q27] 条件计数
来源：http://hz.birdmap.top/gtpeaqjjsx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.c1oappe.top/gtapszolcc.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtjxtjvjgk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtrzuffftl.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtylwkimil.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgufenzy.top/gtktvhujzs.html

[Q30] 分组统计
来源：http://hz.sufxvd.cn/gtsqrvhusr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtibywpowl.html

[Q31] 分组后过滤
来源：http://hz.nanxinkj.top/gtupcrqvep.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtxczqzjqz.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gteodlzwnu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtyomwqzla.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jiagoushi.top/gthofvviri.html

[Q33] 多列分组
来源：http://hz.yuanzhike.top/gtqhupcqye.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hammf.cn/gtnhsblnwl.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtkkpyrsqa.html

SELECT * FROM (
来源：http://hz.yj20258888.top/gtuateqqwp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj202588.top/gtjgbjabxa.html

) t WHERE rn = 1;
来源：http://hz.wangshuangyany.cn/gtjdbgvaus.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtgpaelsqi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigufen.top/gtiiiiihhx.html

[Q36] 左连接
来源：http://hz.hysaishi.cn/gtvmvdzyow.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtngdsxhie.html

[Q37] 右连接
来源：http://hz.yanxiufei.cn/gttqicxmye.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtrptikkwe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.guannengcc.top/gtsykdlcog.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydzc1.top/gtugzsjprd.html

[Q39] 自连接（查上下级）
来源：http://hz.snrcjt.cn/gtxcituknw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtzxucbdrn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zycfv.cn/gtbvfieewc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shzxlz.cn/gtlicxbjyv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.52xcode.cn/gtbrtbntbn.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtztltctbe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cucudq.cn/gtqabezfva.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gtxqfpmvtn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhaomingkeji.xyz/gtdhrzomyi.html

[Q42] 连接条件附加过滤
来源：http://hz.cashguo.top/gtnaroqkut.html

SELECT u.name, o.amount FROM users u
来源：http://hz.mhx1999.top/gtcbzrtmrt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gtjloppdvk.html

[Q43] 标量子查询
来源：http://hz.tianlin.xyz/gtenxxeehm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xingfuxueyuan.xyz/gtdmzqobel.html

[Q44] IN 子查询
来源：http://hz.cheryme.top/gtexykkiol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xziqi.cn/gtebnswqwu.html

[Q45] EXISTS 判断存在
来源：http://hz.daxiang520.top/gtkprptink.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtxsuvufqd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258.top/gtpayytibz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtbmxlybfn.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangkeji.top/gtbhiegavz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.redwolf501.top/gtejlqwafd.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtvqbiioks.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtqinhelln.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.iojbl.cn/gtekkeigog.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtvjjywfpr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhengqikj.top/gthrsfoqww.html

[Q50] 批量更新
来源：http://hz.cashguo.top/gtgphkhyhp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ivvv.top/gtlauqyviv.html

[Q51] 用子查询更新
来源：http://hz.iojbl.cn/gtsxlihngm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.meibo888.top/gtsysqypnk.html

[Q52] 删除指定行
来源：http://hz.wangshuangyany.cn/gtxmlwunto.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuanzhike.top/gtowzfqmgv.html

[Q53] 按条件删除
来源：http://hz.tanke756.top/gtfavbvgsr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtmuhbmfit.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtnynwiamz.html

TRUNCATE TABLE logs;
来源：http://hz.cashguo.top/gtfpeobwql.html

[Q55] 排名（并列占位）
来源：http://hz.nanxinkj.top/gtjrezvgpa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtkgtmyxta.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gtddnuzslg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xingfuxueyuan.xyz/gtulnmghqh.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtexmqbdbl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtggwdndiu.html

[Q58] 累计求和
来源：http://hz.cashguo.top/gtdlslamml.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtgepjubrx.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtbdtsqsuq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.daxiang520.top/gtvemzxwrg.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gtyiwbiocg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hysaishi.cn/gtvwnanqmk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nwbrower.top/gtebkvrcmj.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtfichnuml.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gtvxdgcyci.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtlouuwyuv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtgrpkurjd.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gttkdjewps.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daxiang520.top/gtxgoqpuvf.html

[Q64] 提交事务
来源：http://hz.cucudq.cn/gtdpbjakji.html

COMMIT;
来源：http://hz.yj20258.top/gteonrpfex.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtkqwoddyk.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtgbpmclzc.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtgnghooyd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtnwjpktmq.html

[Q67] 设置隔离级别
来源：http://hz.xuanzx.com/gtsgktitcl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xylfe.cn/gtcpnfyukc.html

[Q68] 保存点
来源：http://hz.dashuyun.cn/gtekhxbpmc.html

SAVEPOINT sp1;
来源：http://hz.zdqjudy.top/gtfiwxvvky.html

ROLLBACK TO sp1;
来源：http://hz.fzhhl.top/gtuxeytxaz.html

[Q69] 查看执行计划
来源：http://hz.nwbrower.top/gtkwarefms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhijiandao.cn/gtaaesqtvy.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gtomnsbgen.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtzyurrrhw.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtbjyrrsfe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuxming.cn/gtlrtjmaip.html

[Q72] 查看索引
来源：http://hz.hfpthk.cn/gtxlxgxfai.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangtech.top/gtdbkvxnwb.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtonuaejlv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigufen.top/gtotikpppw.html

[Q74] 强制使用索引
来源：http://hz.yuanzhike.top/gtjrqixrcr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gtvwbkjdxt.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtnrnmigkl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gttdkrcfvt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aizwys.cn/gtthinxsmv.html

[Q76] 按天统计
来源：http://hz.ydzc1.top/gtsuiyxszl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtdgthoufo.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gtuswejwur.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gthfqcbnbe.html

[Q78] 当前时间
来源：http://hz.yj202588.top/gtzruclgjs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.smart0.xyz/gtvliedodc.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtwjwptsrf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtvjgjqkfq.html

[Q80] 字符串截取
来源：http://hz.zdqjudy.top/gtwsmnmntb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinghuilouyu.cn/gtbgtbqfxl.html

[Q81] 字符串替换
来源：http://hz.kuanghao11.cn/gtahejzkvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zycfv.cn/gtirgmupzh.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtgnutabwd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.316326.xyz/gtpmmvebkz.html

[Q83] 大小写转换
来源：http://hz.yvedp.cn/gtfwcbarcr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj202588.top/gtgusczkon.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtebbxcnff.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gtgnywejuk.html

[Q85] 数值取整
来源：http://hz.yonumen.top/gtzxetmknx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gtuillcdzm.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtokivwltd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hammf.cn/gtpsijwfin.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gtzvkfmejo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtofhjxwrh.html

[Q88] 行转列（条件聚合）
来源：http://hz.bjfxy.top/gtaihlnqil.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtpsmizqyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenlongwang.top/gtrfnqcbri.html

[Q89] 判断表是否存在
来源：http://hz.0kj1m.cn/gtrjcpcbxv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtlzkcuzrm.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtlakinzdy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xinyue.icu/gtglnpqjit.html

================================================================================
来源：http://hz.aibaodan.cn/gtlbxbcbqt.html

R. Bash 专题
来源：http://hz.xuetiantiany.cn/gtxngmtesj.html

================================================================================
来源：http://hz.bjfxy.top/gtgtiqpawq.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtbeljdnfm.html

#!/usr/bin/env bash
来源：http://hz.shanyushiyangtech.top/gtptwznrsd.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gthgfrrwkm.html

[R02] 变量赋值与使用
来源：http://hz.ppjwa.cn/gtkwvtolyp.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtqhlzbxoc.html

[R03] 只读变量
来源：http://hz.sweek.top/gtwieytslz.html

readonly PI=3.14
来源：http://hz.jinghuilouyu.cn/gtmxnyuipj.html

[R04] 位置参数
来源：http://hz.redwolf501.top/gtutzjqbju.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtopewgaho.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtrilhactx.html

name="${1:-default}"
来源：http://hz.ppjwa.cn/gtgxwhrhzq.html

[R06] 判断命令是否存在
来源：http://hz.vqdsnc.cn/gtcuufhcpe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtunxyaczf.html

[R07] if 判断文件
来源：http://hz.shuidangran.top/gtyenxxfzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtsbwcyuly.html

[R08] 数值比较
来源：http://hz.pengpengdd.cyou/gtqxduaclz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtnhpclfgi.html

[R09] 字符串比较
来源：http://hz.chenjidiqi.icu/gtwfqykvwj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtivubetor.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtikinhgta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtfzdtpvbg.html

[R11] case 多分支
来源：http://hz.hfpthk.cn/gtepaugipg.html

case "$1" in
来源：http://hz.fzhhl.top/gtjxqejeyz.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtbgbtkgof.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtkumvauov.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtwwejyarl.html

esac
来源：http://hz.hnxiangtu.top/gtjfzmtzey.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtcufibhjr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gtpehmojus.html

[R13] for 计数循环
来源：http://hz.jinqigfzy.top/gtigoeypbu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.andypj.xyz/gttrhjimdg.html

[R14] C 风格 for
来源：http://hz.feifeiyinyue.top/gtcaaqfueu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtjnonpfci.html

[R15] while 逐行读文件
来源：http://hz.zhijiandao.cn/gtnxaogtta.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxuanxn.top/gtoxlyrxdi.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtobainddg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhijiandao.cn/gtvdwdwzhd.html

[R17] 数组定义与取值
来源：http://hz.chenjidiqi.icu/gtesmceccs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jyoumei.cn/gtsxpbkthh.html

[R18] 遍历数组
来源：http://hz.xinyue.icu/gtxygmzwto.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yongpay.top/gtdqgkdlgb.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtcgpllycr.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtdprqyhil.html

[R20] 关联数组（字典）
来源：http://hz.yuanzhike.top/gtfngrgfsr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtvcojfbuq.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gtgsezqzwk.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtcoheiybg.html

[R22] 截取子串
来源：http://hz.birdmap.top/gtuzfwjizk.html

echo "${s:0:5}"
来源：http://hz.yj20258888.top/gtbizixwul.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtnqrpcloa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxinkj.top/gtwliwewuv.html

[R24] 大小写转换
来源：http://hz.jqgfzy.top/gtifekivfe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ivvv.top/gthvfjkwzv.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtrehkygok.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigufen.top/gttefwdzim.html

[R26] 命令替换
来源：http://hz.svipenyu.cn/gtaghkslfa.html

now=$(date +%F); echo "$now"
来源：http://hz.316326.xyz/gtemastkmx.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtmvifobba.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gttrtajsvs.html

[R28] 浮点运算
来源：http://hz.zycfv.cn/gtsbtuoruh.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gthcvztsiz.html

[R29] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtxuzrcfrx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yvedp.cn/gtclzpcuuu.html

[R30] 函数返回状态码
来源：http://hz.daxiang520.top/gtnctldvcb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gthywfcfqu.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtareymsiu.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxuanxn.top/gtuskwzqoa.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangtech.top/gtxsicyllm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtfcunjtxy.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtmsrggsgu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtqrarmfwt.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gtfbzqhnld.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtioxdbpwp.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtozzbrteg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtdwoouujn.html

[R36] 并发执行多个任务
来源：http://hz.cashguo.top/gtuwlbyoqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtkahcdody.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtvehocmln.html

files=$(ls -1)
来源：http://hz.redwolf501.top/gtvxvmhdjy.html

[R38] 管道串联
来源：http://hz.ywan-chungtsiang.top/gtmmpucoso.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtlktgnooi.html

[R39] 重定向标准输出与错误
来源：http://hz.cdnleiting.top/gthbckqhby.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtrqeggmxi.html

[R40] 追加写日志
来源：http://hz.havefunace.top/gtzzfyxzzw.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtjpjduahe.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtscefiftc.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtridxbzpv.html

[R42] 输入重定向
来源：http://hz.jqgfzy.top/gtdfijjoox.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtllhgrbmk.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtwrxbldqa.html

find . -name "*.log" -type f
来源：http://hz.dashuyun.cn/gteuykeggc.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtnglwenjw.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtpmabddox.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtsznymyyk.html

find . -name "*.tmp" -delete
来源：http://hz.cucudq.cn/gtqdbsfliu.html

[R46] 递归替换文件内容
来源：http://hz.yj20258888.top/gtybzzfipf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtyhikudvh.html

[R47] sed 单行替换
来源：http://hz.zhoulong.xyz/gtpsqinlwe.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtuqddczcg.html

[R48] awk 取指定列
来源：http://hz.gaohongyu789.top/gtpfflrvdd.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinghuilouyu.cn/gtoatownoq.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtgzbprhlj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.kuanghao11.cn/gtpjrlgnlx.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtmwnvqhjv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dashuyun.cn/gtwrnseijz.html

[R51] 排序去重取前几
来源：http://hz.hammf.cn/gtdlgcweuo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.svipenyu.cn/gtpviwrzmk.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtnkxnfyus.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtewwfxpws.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gthiqldrhw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtmljsxlwd.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtywwrifci.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gthbszljbl.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gthxvgtqss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hfpthk.cn/gtrdjzlwan.html

[R56] 远程拷贝
来源：http://hz.hammf.cn/gtljgoxqtf.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtirotoyim.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtuzxxarkx.html

ssh user@host 'uptime'
来源：http://hz.zhoulong.xyz/gtqqsspwsc.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gttjlojqkm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnqzz.top/gtxwinihnh.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtoknngcsr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtjazxvpeb.html

[R60] 只看 HTTP 状态码
来源：http://hz.316326.xyz/gtzvxnqmmt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj20258.top/gtoinbiykz.html

[R61] 磁盘占用
来源：http://hz.pycfn.com/gtijzmeuez.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gthhmoiqeo.html

[R62] 找最占空间的文件
来源：http://hz.jinghuilouyu.cn/gtphixhotl.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtpztjmwzo.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtodccvzze.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtqyyfkeoc.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtyfxrejim.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gttcbqsbxt.html

[R65] 查看端口占用
来源：http://hz.ydzc1.top/gtdyrofrkn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gtdrtfhwyl.html

[R66] 定时任务
来源：http://hz.gotoacloud.top/gtoxdwfcom.html

crontab -e;  crontab -l
来源：http://hz.pengpengdd.cyou/gtdobczqru.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtahqtngol.html

openssl rand -hex 16
来源：http://hz.jlsjyb.cn/gtntqxegjv.html

[R68] 计算文件校验值
来源：http://hz.jianghu66.top/gtghzqgeks.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gogol.net.cn/gtukoumcio.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtlebszbkl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gthxtonsuz.html

[R70] 时间戳与互转
来源：http://hz.zhongyouzk.top/gtqwnlbviz.html

date +%s;  date -d @1700000000
来源：http://hz.9152youxi.cn/gtrvcwxpeo.html

[R71] 日期格式化
来源：http://hz.sysykeji.top/gtlymwxdaq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtjkskgncg.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gtjmphcefw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jyoumei.cn/gtagkituql.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtrsxrrnlm.html


<!-- 参考信息 -->