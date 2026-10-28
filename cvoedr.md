代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ivvv.top/gtylfiwhyt.html

[Q22] 排序
来源：http://hz.wangshuangyany.cn/gtbkjukyxj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gtpjwqovft.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gtyporjqcf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xuetiantiany.cn/gtnokbafsl.html

[Q24] 去重
来源：http://hz.yj20258.top/gtwpyjwpgx.html

SELECT DISTINCT city FROM users;
来源：http://hz.tian-w.cn/gtwaglzoat.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtaumgbura.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cucudq.cn/gtfqfyzjfh.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gteooftdao.html

SELECT COUNT(*) FROM users;
来源：http://hz.hnqzz.top/gtqdabhwvq.html

[Q27] 条件计数
来源：http://hz.meibo888.top/gtspdgjkzx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cashguo.top/gtxwobluag.html

[Q28] 求和与平均
来源：http://hz.chenzaomai.com/gthkgymsec.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gthqyduqbp.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtokzvcqyd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gtjrzbvdnh.html

[Q30] 分组统计
来源：http://hz.chenlongwang.top/gtphouwzeg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtwwqkgolt.html

[Q31] 分组后过滤
来源：http://hz.c1oappe.top/gtmmuerrfa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yuanzhike.top/gtiovsuhqz.html

[Q32] 分组拼接字符串
来源：http://hz.yuxming.cn/gtfgccbght.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtjrydcoys.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtlkbejwyd.html

[Q33] 多列分组
来源：http://hz.chenlongwang.top/gtdrayomtc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtpgepcwmd.html

[Q34] 每组取第一条
来源：http://hz.xingfuxueyuan.xyz/gtpzwayuhu.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtdsmtyfzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtsetilxsn.html

) t WHERE rn = 1;
来源：http://hz.mhx1999.top/gtfcprliwj.html

[Q35] 内连接
来源：http://hz.chenlongwang.top/gtzlkgjuqf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtxwyakhjj.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtoqvcqjdm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtnwqshyaz.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtmxaccqtu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jianghu66.top/gtclqoedlc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtqmspwnch.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daxiang520.top/gtrekzecok.html

[Q39] 自连接（查上下级）
来源：http://hz.guowangkeji.top/gttrdnhuah.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shuidangran.top/gtjvzwjsru.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cqqwz.cn/gtolwtqrlg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.andypj.xyz/gtyxcxfxdk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtdbxiqwkl.html

[Q41] 多表连接
来源：http://hz.yanxiufei.cn/gtfxbsfisj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxinkj.top/gtksnuacwk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gaohongyu789.top/gtksrcurog.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fengsongda.top/gtxqbxoifh.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gtanrriixr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gtixbmckxf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtxtdhpgcs.html

[Q43] 标量子查询
来源：http://hz.c1oappe.top/gtxaumpola.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tanke756.top/gtjlvwrqef.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtkijeghll.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cqqwz.cn/gtqmlbfrne.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtqrcorlgh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtqyebxjzx.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.bjfxy.top/gtnpgwiskc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.vqdsnc.cn/gtlghhhdoe.html

[Q47] 与平均值比较
来源：http://hz.jianghu66.top/gtajeyumkx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.iojbl.cn/gtkullzugl.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gthwglkkiu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtzyfbtcqz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.vqdsnc.cn/gtkdcznzoh.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gttngtfhqj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtrsayiwrm.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtzngmtwpz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtarryypwh.html

[Q51] 用子查询更新
来源：http://hz.bjfxy.top/gtlxveqrdt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.guowangkeji.top/gtrdmdlfvl.html

[Q52] 删除指定行
来源：http://hz.jqgufenzy.top/gtdtkecfgv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuanzhike.top/gtwfewtuif.html

[Q53] 按条件删除
来源：http://hz.wangdashe.top/gtwnuyimds.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gotoacloud.top/gtdqceawgq.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtathkpdra.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gttrqlllne.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtinpterxh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtqrpzahfa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xinyue.icu/gttxwvfepx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gaohongyu789.top/gtfjumgozs.html

[Q57] 行号
来源：http://hz.fengsongda.top/gtkojlfkqt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hongshengwenyu.top/gtjjzgknzu.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtppxokunp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yuxming.cn/gtjpcyxnfe.html

[Q59] 分组内累计
来源：http://hz.hysaishi.cn/gtxinzjlls.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hfpthk.cn/gtvnmugeas.html

[Q60] 取上一行 / 下一行
来源：http://hz.vqdsnc.cn/gtinnvmjks.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yvedp.cn/gtgxrverjp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.nanxuanxn.top/gtxrsvctnv.html

[Q61] 移动平均
来源：http://hz.havefunace.top/gtitefozua.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gttvohjlkg.html

[Q62] 分组占比
来源：http://hz.yongpay.top/gthcovkjpi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtmemwjdwk.html

[Q63] 开启事务
来源：http://hz.hysaishi.cn/gtevmqnnrt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aibaodan.cn/gtbwbibizl.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtekukkxzh.html

COMMIT;
来源：http://hz.ydjk.org.cn/gtamgoaclp.html

[Q65] 回滚事务
来源：http://hz.sysykeji.top/gtbxkylmic.html

ROLLBACK;
来源：http://hz.quarkkingdee.top/gtywgwndny.html

[Q66] 行锁查询
来源：http://hz.pycfn.com/gtfedltlhs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtquzjqrls.html

[Q67] 设置隔离级别
来源：http://hz.ppjwa.cn/gtzwhcazwc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gttlpdjyut.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gtbzkqiemy.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtkwcwukwv.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangtech.top/gtvcmrkuui.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtabykdusb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sweek.top/gtqajedetv.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gthlsclrmg.html

ANALYZE TABLE users;
来源：http://hz.c1oappe.top/gtteivpvrv.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtatfncmqb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtujpddetk.html

[Q72] 查看索引
来源：http://hz.xuetiantiany.cn/gtadfgsvnq.html

SHOW INDEX FROM users;
来源：http://hz.hammf.cn/gtdxjmutxa.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtwwmlczer.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.c1oappe.top/gtibfcbvke.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtpmxiofvr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gteemwvhfh.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtlpjrqbtg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gtbgwbbfxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtgdejucvf.html

[Q76] 按天统计
来源：http://hz.zhengqikj.top/gtytgkcdhn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ywan-chungtsiang.top/gtxbvnfjfm.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtfnkyqadl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gtfvcrqzgk.html

[Q78] 当前时间
来源：http://hz.fengsongda.top/gtcqlzaazo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtwwtcvnze.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtgbygzyvf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtxghcjlkf.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gtrlxyevcm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dashuyun.cn/gtkmktdnlm.html

[Q81] 字符串替换
来源：http://hz.havefunace.top/gtekduxkks.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtfxkskhyd.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtcvwykbdh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtabdbvtze.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtsazhwadi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.snrcjt.cn/gtducfmnzl.html

[Q84] 去除首尾空格
来源：http://hz.ivvv.top/gtktkfiggd.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gtvyfwlyhx.html

[Q85] 数值取整
来源：http://hz.jinqigfzy.top/gtpgtbqcid.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dashuyun.cn/gtkaxcuvzs.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtwpobyfdh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sweek.top/gtwmmnuqnq.html

[Q87] JSON 字段做条件
来源：http://hz.zdqjudy.top/gtuysbvvof.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnxiangtu.top/gtfawncyiz.html

[Q88] 行转列（条件聚合）
来源：http://hz.ehwqpu.com/gtdqgqzfis.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxinkj.top/gtpyfssrfe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.316326.xyz/gtcemcyhpq.html

[Q89] 判断表是否存在
来源：http://hz.bjfxy.top/gttxedriii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtveywpdqx.html

[Q90] 生成序号列
来源：http://hz.52xcode.cn/gtkzyjokei.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuxming.cn/gtzkneccim.html

================================================================================
来源：http://hz.shzxlz.cn/gthurivdgw.html

R. Bash 专题
来源：http://hz.wangdashe.top/gtgmlamfey.html

================================================================================
来源：http://hz.hammf.cn/gtymofdcun.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gtzbvhbtub.html

#!/usr/bin/env bash
来源：http://hz.hfpthk.cn/gtmekvripk.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gtykiyyvjn.html

[R02] 变量赋值与使用
来源：http://hz.316326.xyz/gtgxoldipg.html

name="Tom"; echo "$name"
来源：http://hz.nwbrower.top/gtugfbfqzv.html

[R03] 只读变量
来源：http://hz.havefunace.top/gtyxpvwqdl.html

readonly PI=3.14
来源：http://hz.shanyushiyangtech.top/gtskbhdqgh.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtnzorztqh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sufxvd.cn/gtceeffjrg.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gthmspnlcu.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtomgawobj.html

[R06] 判断命令是否存在
来源：http://hz.chenjidiqi.icu/gtlysrhsqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtxkbqmaho.html

[R07] if 判断文件
来源：http://hz.zhijiandao.cn/gtltsenhvk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jqgfzy.top/gtfpzklrim.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtmvqupudl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gaohongyu789.top/gtrvxtxnmv.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gtbafmhkbk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhoulong.xyz/gteoiklxte.html

[R10] 正则匹配
来源：http://hz.svipenyu.cn/gturumiowo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtnfmwlmio.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtxtufszql.html

case "$1" in
来源：http://hz.hysaishi.cn/gtgvcjxliy.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gtknbjwpys.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtgwbhufcp.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtgnbhjnxs.html

esac
来源：http://hz.0kj1m.cn/gtkcgowmsm.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtbxgyfvgc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtwojgabsg.html

[R13] for 计数循环
来源：http://hz.jqgufenzy.top/gthmzkjvpe.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gtjedyztvu.html

[R14] C 风格 for
来源：http://hz.mhx1999.top/gtyekzxlix.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtxkbhwygy.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtshyfpsyt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtifrhlshl.html

[R16] until 等待条件
来源：http://hz.yueranfly.top/gtgpcbnnmn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gtrosxgena.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtjounczem.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.havefunace.top/gtfxbusyab.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtzhupplar.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cdnleiting.top/gthkzcytnj.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtlecipgpv.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtdajuytjn.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtenuxtxlb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydzc1.top/gtxigyzvhc.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtnefgeikr.html

echo "${#s}"
来源：http://hz.jiagoushi.top/gtnrifvsjj.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtrbdmpxkl.html

echo "${s:0:5}"
来源：http://hz.ywan-chungtsiang.top/gtunwonejz.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gtufrgxhjr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gterxwbfme.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtouixfhoi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gzhubu.top/gtdhzwkbar.html

[R25] 去后缀 / 去前缀
来源：http://hz.chenlongwang.top/gtxcqibvyp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hongshengwenyu.top/gtahtgwaml.html

[R26] 命令替换
来源：http://hz.yj20258.top/gtpcvkatsj.html

now=$(date +%F); echo "$now"
来源：http://hz.xziqi.cn/gtokfpocfs.html

[R27] 算术展开
来源：http://hz.ydjk.org.cn/gtbgverjki.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtexrtnpog.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtynyikzvw.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtcnjpsqvw.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtgblgzzky.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtbilghpvh.html

[R30] 函数返回状态码
来源：http://hz.jinghuilouyu.cn/gthlscwptt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtkrduuybd.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtcyeijikb.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtkxagjdfs.html

[R32] 参数个数校验
来源：http://hz.svipenyu.cn/gttlwwhyxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.9152youxi.cn/gtfnvfyyuo.html

[R33] 捕获错误并提示行号
来源：http://hz.guowangkeji.top/gtoefuuhjp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtmucdmwtl.html

[R34] 退出时清理
来源：http://hz.fzhhl.top/gtkckbufse.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtbyouywop.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtzldkxfmw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sufxvd.cn/gtwhcabsxb.html

[R36] 并发执行多个任务
来源：http://hz.316326.xyz/gtdnybpxjp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtbzgulckp.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtqlhfxwkj.html

files=$(ls -1)
来源：http://hz.bjfxy.top/gtnlcdxbrd.html

[R38] 管道串联
来源：http://hz.ydjk.org.cn/gttttlxekj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtffqbinlm.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigfzy.top/gtqzaqoist.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtnlxwcdrv.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtluiokxrb.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gtwytvgyky.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtphphwkmb.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtqfcsuwdm.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gtmmorkroj.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtbtcpuqqe.html

[R43] 按名字查找文件
来源：http://hz.guowangkeji.top/gtnveqwtww.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtrbumdkqs.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtiqzukomb.html

find . -mtime -7 -type f
来源：http://hz.cdnleiting.top/gtpraislcc.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtjrzfupxo.html

find . -name "*.tmp" -delete
来源：http://hz.cdnleiting.top/gtqwubafft.html

[R46] 递归替换文件内容
来源：http://hz.hnxiangtu.top/gtghigneuu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fzhhl.top/gtvtbahlgk.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtgplhnoic.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gtjapnsebu.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtajlqmvex.html

awk '{print $1, $3}' a.txt
来源：http://hz.havefunace.top/gtgpjxelbp.html

[R49] awk 带条件
来源：http://hz.shanyushiyangtech.top/gtlvflteot.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj202588.top/gtimnthbuh.html

[R50] awk 求和
来源：http://hz.zhiwuduotai.top/gtnwdhanks.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cdnleiting.top/gtxvcpvpln.html

[R51] 排序去重取前几
来源：http://hz.shangyingyoupin.top/gtgehxsisb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtjvbprkfb.html

[R52] 统计行数
来源：http://hz.sweek.top/gtgseovobc.html

wc -l a.txt
来源：http://hz.redwolf501.top/gttnnwzfid.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258.top/gtwzhpqoqp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtshrqilnb.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtqkmghkno.html

diff a.txt b.txt
来源：http://hz.gogol.net.cn/gtfwggllyr.html

[R55] 压缩与解压
来源：http://hz.yanxiufei.cn/gtsslprgzy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gtkkwnjkji.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtnnlqlglo.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtzwrmnjjl.html

[R57] 远程执行命令
来源：http://hz.havefunace.top/gtxsobvnre.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gtnhpeyrfh.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gttzaqswjl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtevfssagl.html

[R59] 发 POST JSON
来源：http://hz.jiagoushi.top/gtfqcfldgu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ybcxt.top/gtezqvlvfh.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtylgcfbqb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtvropidku.html

[R61] 磁盘占用
来源：http://hz.jinqigufen.top/gtzpgewwzu.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtlzetqmoc.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtzdejskzm.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtjqttilsj.html

[R63] 内存与进程
来源：http://hz.snrcjt.cn/gtnukmhlsa.html

free -h;  ps aux | grep nginx
来源：http://hz.vqdsnc.cn/gtujcadbjp.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtvyuezzcc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtcssjigso.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gtcqyaxtmf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gtwmkkynox.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gtovdfzgdi.html

crontab -e;  crontab -l
来源：http://hz.jianghu66.top/gtxlczaqae.html

[R67] 生成随机十六进制串
来源：http://hz.snrcjt.cn/gteqmnskrl.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtsrxyqhjn.html

[R68] 计算文件校验值
来源：http://hz.cucudq.cn/gtrxhumzkw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gtowuhinex.html

[R69] 生成随机密码
来源：http://hz.jqgfzy.top/gtpdxhyood.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtvhpixrir.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gtngcnaigy.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtjptcasjg.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtxwpfgurs.html


<!-- 参考信息 -->