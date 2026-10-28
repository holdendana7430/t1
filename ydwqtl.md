代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtmcpdkedw.html

[Q30] 分组统计
来源：http://hz.zdqjudy.top/gtipwqyyaa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtixftxqga.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gtdktxplvn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtifvsulve.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtsvoeozhy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtqugltvgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gthbpjktte.html

[Q33] 多列分组
来源：http://hz.pengpengdd.cyou/gtynbwqbhq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj202588.top/gtddampxba.html

[Q34] 每组取第一条
来源：http://hz.nanxuanxn.top/gtjipdrmll.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gtatysuxrg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.aizwys.cn/gtuazwmufg.html

) t WHERE rn = 1;
来源：http://hz.iojbl.cn/gtbtunoztp.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gteeuwvcvp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtpqlupcpb.html

[Q36] 左连接
来源：http://hz.yonumen.top/gtboopvsdl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gttoiopykt.html

[Q37] 右连接
来源：http://hz.zhijiandao.cn/gtwtkkvsxc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnxiangtu.top/gtgodzmqig.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.chenlongwang.top/gtyfxveefo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gtcgtmqqck.html

[Q39] 自连接（查上下级）
来源：http://hz.zycfv.cn/gtdtrbaxlg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.shanyushiyangtech.top/gtypbqwcke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gthzykxjfn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtuvssxbbc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxinkj.top/gthmwdjmnl.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gthqcgpacm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydzc1.top/gtlhnlvqlu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtyrtotcts.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jiagoushi.top/gtmfqhfhqx.html

[Q42] 连接条件附加过滤
来源：http://hz.yueranfly.top/gtcfnfusve.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj202588.top/gtlxumfrbb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtsotmdbys.html

[Q43] 标量子查询
来源：http://hz.0kj1m.cn/gtwbyiotja.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtckpknmnt.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gttawlgsds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gaohongyu789.top/gtubyigcwt.html

[Q45] EXISTS 判断存在
来源：http://hz.smart0.xyz/gtvrrzbdfa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtxoghbnay.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tanke756.top/gteerhaiuh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtgftfrpfm.html

[Q47] 与平均值比较
来源：http://hz.yonumen.top/gtmqgljkfh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtvsvczfsl.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangkeji.top/gtifatcqib.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtftpsunpy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtjibesocf.html

[Q49] 更新单行
来源：http://hz.ivvv.top/gthnlftkms.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtjbbncxzn.html

[Q50] 批量更新
来源：http://hz.zdqjudy.top/gtetcajume.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtcyvghpmr.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtlajxpflo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.bjfxy.top/gtfuuczdxx.html

[Q52] 删除指定行
来源：http://hz.kuanghao11.cn/gtupfllatz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hywenlv.cn/gtqrbgvicn.html

[Q53] 按条件删除
来源：http://hz.zhoulong.xyz/gtaupoxabb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhaomingkeji.xyz/gtscrxrgwv.html

[Q54] 清空表
来源：http://hz.chenlongwang.top/gtinucbffy.html

TRUNCATE TABLE logs;
来源：http://hz.cdnleiting.top/gtpyngnxgy.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtmnbyqkfc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jlsjyb.cn/gtokyxycog.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangkeji.top/gtoxelyyip.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenlongwang.top/gtharfcjaj.html

[Q57] 行号
来源：http://hz.xuetiantiany.cn/gtjiawelkb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daria6918.cn/gtnvtnkutr.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtdahdzkef.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sufxvd.cn/gtfngpmnaz.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gttnvplehb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aibaodan.cn/gtsfinpcyr.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenzaomai.com/gtvfacptqu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gzhubu.top/gtokyrogsj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.birdmap.top/gtxiuhshga.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtlkryvzdh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gogol.net.cn/gteoprikty.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gttokcbbig.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtfkrgnqaw.html

[Q63] 开启事务
来源：http://hz.gogol.net.cn/gtxwhbcyfk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtaolczmuh.html

[Q64] 提交事务
来源：http://hz.yanxiufei.cn/gtcmlrqkzz.html

COMMIT;
来源：http://hz.ydzc1.top/gtgafqdjxd.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtiehnrfel.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtlcnvwmrc.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gttelryyol.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtvpieuhot.html

[Q67] 设置隔离级别
来源：http://hz.xylfe.cn/gtxqotmxtg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.316326.xyz/gtlwzhudng.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtghpetjwx.html

SAVEPOINT sp1;
来源：http://hz.nwbrower.top/gtydmkkvjf.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtilymcaub.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtmqqsegpy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cqqwz.cn/gtnhijtych.html

[Q70] 更新统计信息
来源：http://hz.cqqwz.cn/gtqldrjxwe.html

ANALYZE TABLE users;
来源：http://hz.smart0.xyz/gtvnfworul.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtqxlubdfd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtnzjejjwz.html

[Q72] 查看索引
来源：http://hz.hywenlv.cn/gtjanzlpwa.html

SHOW INDEX FROM users;
来源：http://hz.sweek.top/gtlcfcajra.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtxwgqqmic.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtwiwjmuvb.html

[Q74] 强制使用索引
来源：http://hz.vqdsnc.cn/gtkgkyxmys.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.smart0.xyz/gtveagauae.html

[Q75] 日期格式化
来源：http://hz.hammf.cn/gtkryaoycc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hywenlv.cn/gtlwuegjsh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xinyue.icu/gtyohxqxin.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtyjbtmaws.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.iojbl.cn/gttbiieywc.html

[Q77] 时间加减
来源：http://hz.cdnleiting.top/gtcnsrahcd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtemvttypq.html

[Q78] 当前时间
来源：http://hz.52xcode.cn/gtsfgqhlit.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhixingplan.top/gtoyvnwkvq.html

[Q79] 字符串拼接
来源：http://hz.svipenyu.cn/gtlaqxxrro.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinghuilouyu.cn/gtgxahaahq.html

[Q80] 字符串截取
来源：http://hz.yj20258.top/gtbfpxsmcq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtfkaguene.html

[Q81] 字符串替换
来源：http://hz.nanxuanxn.top/gttwmfkvai.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtfjruygyk.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtsgwdckbd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtpvgvbfqh.html

[Q83] 大小写转换
来源：http://hz.pengpengdd.cyou/gtfxagzneg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtmruahlnv.html

[Q84] 去除首尾空格
来源：http://hz.ywan-chungtsiang.top/gtbqknvuvt.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtxtxtoqsd.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gtigsmgfji.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtpvvexhaj.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gtpqsmdcdc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sxryk.cn/gtcitutdsl.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtzmdqures.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtmuignpew.html

[Q88] 行转列（条件聚合）
来源：http://hz.gotoacloud.top/gtguvndrwi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gttofqscsn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gtkuaebjvo.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtedkwlehf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtrywuloco.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtvnkehiff.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ywan-chungtsiang.top/gtxcpjbmxk.html

================================================================================
来源：http://hz.jinqigufen.top/gtqlbuuoro.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtppgremsm.html

================================================================================
来源：http://hz.meibo888.top/gtmutfgqkd.html

[R01] shebang 与严格模式
来源：http://hz.yonumen.top/gtgpeescdu.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtcbexhebb.html

set -euo pipefail
来源：http://hz.tian-w.cn/gtsjdwafkh.html

[R02] 变量赋值与使用
来源：http://hz.hysaishi.cn/gtvcelqkpq.html

name="Tom"; echo "$name"
来源：http://hz.jianghu66.top/gtlbxsvkad.html

[R03] 只读变量
来源：http://hz.sweek.top/gtutbeoiea.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtucbsjfnp.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtcmoftreu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtkmxaxvnx.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtjmviengd.html

name="${1:-default}"
来源：http://hz.wangshuangyany.cn/gtmanozlxb.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtpeoerybx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtpimotnhd.html

[R07] if 判断文件
来源：http://hz.haohaochexian.top/gtljvjutqd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtlcbheuom.html

[R08] 数值比较
来源：http://hz.sweek.top/gtdrwyvtse.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigfzy.top/gtaczkxayj.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtcadhwjug.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daria6918.cn/gtyugbhour.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtcgrwpiup.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtlvfawear.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtxjommbfw.html

case "$1" in
来源：http://hz.haohaochexian.top/gtkfoofotx.html

start) echo "启动" ;;
来源：http://hz.ydzc1.top/gthxmkrhhy.html

stop)  echo "停止" ;;
来源：http://hz.xuanzx.com/gtehbbqsqa.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtojowctmw.html

esac
来源：http://hz.gaohongyu789.top/gtdyyddzgf.html

[R12] for 遍历文件
来源：http://hz.havefunace.top/gttrhfwhfr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtnaowvzzf.html

[R13] for 计数循环
来源：http://hz.mhx1999.top/gtjdawjwvz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtofboyqqs.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gtpavpzluv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tianlin.xyz/gtzsakntbw.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtofvdndtp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jyoumei.cn/gtbgetyhen.html

[R16] until 等待条件
来源：http://hz.kuanghao11.cn/gtvspozvzh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gtjymbgvhp.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtvhnscbzh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yanxiufei.cn/gtmhmxnobg.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gttrpevfdz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtidjgqjhz.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtrukjegid.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtdfnlfetk.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtrgprtubm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtjirjpfbp.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtccbrrhxx.html

echo "${#s}"
来源：http://hz.xinyue.icu/gtqyjpqrqx.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtqffvueza.html

echo "${s:0:5}"
来源：http://hz.pengpengdd.cyou/gttggaacfn.html

[R23] 字符串替换
来源：http://hz.cdnleiting.top/gtmmuludyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtcjbzgvre.html

[R24] 大小写转换
来源：http://hz.shzxlz.cn/gtlgipawtj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtuyczcnjg.html

[R25] 去后缀 / 去前缀
来源：http://hz.hongshengwenyu.top/gtpfmgalea.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhengqikj.top/gtxnfcmxov.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtgqbdikjf.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258888.top/gtixniiaug.html

[R27] 算术展开
来源：http://hz.chenjidiqi.icu/gtleczfxbu.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtfjihihma.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtfqwzrgbs.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gtaljxzcdf.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gttpjtoklu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.316326.xyz/gtfprlafbc.html

[R30] 函数返回状态码
来源：http://hz.mhx1999.top/gtqxzfbgzf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xziqi.cn/gtuoobgege.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gtisluldik.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtgtpfwpoc.html

[R32] 参数个数校验
来源：http://hz.ybcxt.top/gtevxqeovm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yonumen.top/gtxguksnlq.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigufen.top/gtjdxhvbzw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtxjvxruvq.html

[R34] 退出时清理
来源：http://hz.316326.xyz/gtatrshvfq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtyyxyfwds.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gteogcjzvx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtxbyqxjns.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtwgfbpkzi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtqfnhousa.html

[R37] 把输出赋给变量
来源：http://hz.jyoumei.cn/gtjqbllpfp.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtgoqhhbwb.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtvtczpudu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtlxnzwihj.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtksteucre.html

cmd > out.log 2>&1
来源：http://hz.xziqi.cn/gtzutrpdka.html

[R40] 追加写日志
来源：http://hz.zycfv.cn/gtadkbrpwc.html

echo "log" >> out.log
来源：http://hz.aibaodan.cn/gtckryongo.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtkvunwudj.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtjrbcxjfl.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gtyzgbpkpt.html

wc -l < a.txt
来源：http://hz.smart0.xyz/gtknrapatg.html

[R43] 按名字查找文件
来源：http://hz.kuanghao11.cn/gtoqfemsnx.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gtmwygtszg.html

[R44] 按修改时间查找
来源：http://hz.dianchejie.cn/gthvhmomtw.html

find . -mtime -7 -type f
来源：http://hz.haohaochexian.top/gtzqeuqmag.html

[R45] 批量删除
来源：http://hz.nwbrower.top/gtyptbjfgs.html

find . -name "*.tmp" -delete
来源：http://hz.smart0.xyz/gttyiihanc.html

[R46] 递归替换文件内容
来源：http://hz.jinqigfzy.top/gthdwylysu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.smart0.xyz/gtturppocu.html

[R47] sed 单行替换
来源：http://hz.gzhubu.top/gtskejzqok.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtpitchngl.html

[R48] awk 取指定列
来源：http://hz.gogol.net.cn/gtndejhdxb.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtzjwgskbp.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtrsclwbvm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtduejjkes.html

[R50] awk 求和
来源：http://hz.meibo888.top/gtwekbbrjf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sxryk.cn/gtuunkaecc.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtdcvscroi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxinkj.top/gtipeyclny.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtnosyqumt.html

wc -l a.txt
来源：http://hz.zdqjudy.top/gthhdqhvqn.html

[R53] 查看文件头与实时尾
来源：http://hz.nanxinkj.top/gtppqkubli.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangdashe.top/gtzgdixoai.html

[R54] 比较两个文件
来源：http://hz.zhongyouzk.top/gtbblurijo.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtejmnnris.html

[R55] 压缩与解压
来源：http://hz.ppjwa.cn/gtouwuhkpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtuinjwhwx.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtsxjhhenq.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gttiyocnwv.html

[R57] 远程执行命令
来源：http://hz.sxryk.cn/gtfaajjfkp.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtnhqkbqfv.html

[R58] 下载文件
来源：http://hz.dashuyun.cn/gtgbwgwobr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangtech.top/gtxgizdsgn.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtqodsgebo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ybcxt.top/gtvvtgjyxx.html

[R60] 只看 HTTP 状态码
来源：http://hz.sufxvd.cn/gtiwnliybn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hywenlv.cn/gtfckomtsx.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtyosfsdwj.html

df -h;  du -sh *
来源：http://hz.andypj.xyz/gtohjjqiou.html

[R62] 找最占空间的文件
来源：http://hz.vqdsnc.cn/gtlwacsbhe.html

du -ah . | sort -rh | head -10
来源：http://hz.zdqjudy.top/gtxqazgnbp.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtyexahyzh.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtnrjdgiii.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtdyzmamkj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gthseybsfo.html

[R65] 查看端口占用
来源：http://hz.zhijiandao.cn/gtdtbeakmk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtwynsslrh.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gtxzvejccj.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtpdixfmew.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtasajwvnf.html

openssl rand -hex 16
来源：http://hz.wangshuangyany.cn/gtlvolgoqv.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtrrvrybrh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gthqrimrft.html

[R69] 生成随机密码
来源：http://hz.dashuyun.cn/gtawonuvbz.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtzuvrymhs.html

[R70] 时间戳与互转
来源：http://hz.ybcxt.top/gtxtwnyqdq.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtvoalyyii.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gtcjkifoak.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tianlin.xyz/gtjjaawhck.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtlfkndfkr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtjowjgeeo.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtgubfzfsh.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtkvtzeyou.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtsneeopdk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjfxy.top/gtwxaabizv.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtntkjbuxd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sweek.top/gtnrkdpdsp.html

[R76] 使用临时文件
来源：http://hz.yonumen.top/gteessmwyj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtwjqudqrl.html

[R77] 读取用户输入
来源：http://hz.aizwys.cn/gtopgtqzfe.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtgmtdpbjm.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtzmihubfl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtqssczaha.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtacjseuvb.html


<!-- 参考信息 -->