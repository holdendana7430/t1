代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pycfn.com/gtrdczcxip.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtwoeofjjz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtjimqytzq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.bjfxy.top/gtdseizhvd.html

[Q33] 多列分组
来源：http://hz.0kj1m.cn/gtiykalzmf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jlsjyb.cn/gtmxuehtyq.html

[Q34] 每组取第一条
来源：http://hz.zhijiandao.cn/gtjkffnhmg.html

SELECT * FROM (
来源：http://hz.aizwys.cn/gtwnuzvren.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtksxjdpaa.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtdjqarqzr.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtoqsizcta.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtimubpajp.html

[Q36] 左连接
来源：http://hz.xinyue.icu/gtkitfgjdv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtvdwunfko.html

[Q37] 右连接
来源：http://hz.ybcxt.top/gthkymrapt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj202588.top/gtwbffssup.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gtprorfjmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cheryme.top/gtwjvwndxt.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtgqmrniuh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtpzahgdxb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtunxcyejd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tian-w.cn/gtzfwghauy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.0kj1m.cn/gtyctvvokr.html

[Q41] 多表连接
来源：http://hz.yonumen.top/gtcvjtnege.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ybcxt.top/gtogfktyzr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gogol.net.cn/gtlrfsgckx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtkdxzdrve.html

[Q42] 连接条件附加过滤
来源：http://hz.jyoumei.cn/gttptflvdy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenjidiqi.icu/gtjohumdff.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.redwolf501.top/gtybjvdgjn.html

[Q43] 标量子查询
来源：http://hz.xingfuxueyuan.xyz/gtxaxlsiwt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ywan-chungtsiang.top/gttrrfelpq.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gtgjuzcjot.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtxywnvgps.html

[Q45] EXISTS 判断存在
来源：http://hz.tanke756.top/gtdlwtjgwz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtcmcupjby.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtyfjuoxmn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtckxeubue.html

[Q47] 与平均值比较
来源：http://hz.ivvv.top/gtynyuexhu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtdwcyuubx.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gthhnuzknx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gttysolcvv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sufxvd.cn/gtzxshsndz.html

[Q49] 更新单行
来源：http://hz.ywan-chungtsiang.top/gthdykxrrj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtfwuavjjb.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gtfegajjvl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jiagoushi.top/gtdtpsscxg.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtriuqvods.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.quarkkingdee.top/gtumcpewum.html

[Q52] 删除指定行
来源：http://hz.xingfuxueyuan.xyz/gtwiyrxfoy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hfpthk.cn/gtnpivqmam.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtrrlebuug.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gtttlpoboa.html

[Q54] 清空表
来源：http://hz.dianchejie.cn/gtgbkcolsl.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gttvfrqazh.html

[Q55] 排名（并列占位）
来源：http://hz.sufxvd.cn/gtflasnoaf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtjiqxolji.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangdashe.top/gtefqjyvtp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gtargxwiwp.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtodfuhvtf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hongshengwenyu.top/gtodsnypgi.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gtmysqgoeg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gttemfmyrc.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtnecpplzo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtguokwgya.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtisankmax.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtlujmeqbc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtmgapuqay.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtcpomriap.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtnrrcxzed.html

[Q62] 分组占比
来源：http://hz.yueranfly.top/gtpisbgbby.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtfkpnfmca.html

[Q63] 开启事务
来源：http://hz.snrcjt.cn/gtbgamsseb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtmzwmxvom.html

[Q64] 提交事务
来源：http://hz.chenjidiqi.icu/gtefhrzzuq.html

COMMIT;
来源：http://hz.yangfankeji.com/gtisqindxv.html

[Q65] 回滚事务
来源：http://hz.daria6918.cn/gtxouwqbzz.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtcdiqbsps.html

[Q66] 行锁查询
来源：http://hz.yuanzhike.top/gtodskrits.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuxming.cn/gthnwpjfwn.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtcxnxjlpj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jianghu66.top/gtaujqljcg.html

[Q68] 保存点
来源：http://hz.xuetiantiany.cn/gtuirtkuuz.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtymylwlyl.html

ROLLBACK TO sp1;
来源：http://hz.ydjk.org.cn/gtczflxbqv.html

[Q69] 查看执行计划
来源：http://hz.yanxiufei.cn/gtsujuwbvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gzhubu.top/gtxeirczdp.html

[Q70] 更新统计信息
来源：http://hz.chenlongwang.top/gthdkvjgjb.html

ANALYZE TABLE users;
来源：http://hz.ydzc1.top/gtbracazmk.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtykiggfty.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtytelcmdc.html

[Q72] 查看索引
来源：http://hz.yj202588.top/gtxnhszdds.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtdorttxbd.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gtzrvgngfn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtycultorm.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtkmkizjsu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shzxlz.cn/gtrxpkxtun.html

[Q75] 日期格式化
来源：http://hz.havefunace.top/gtxlkpdiss.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.daxiang520.top/gtrjelwcww.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258.top/gtlzjnzmhr.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtsywtghhh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtpelkpzud.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtvovhovvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.mhx1999.top/gtvpxggptq.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtaihtoqpm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guannengcc.top/gtngccldar.html

[Q79] 字符串拼接
来源：http://hz.tianlin.xyz/gtgpzpifaa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gteieyddfb.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtaqmwnvpz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shuidangran.top/gtlykqxnid.html

[Q81] 字符串替换
来源：http://hz.hnxiangtu.top/gtcubcyoxn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shuidangran.top/gtzykpdfxk.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gtncvznrht.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenlongwang.top/gtciwiiqmt.html

[Q83] 大小写转换
来源：http://hz.zhoulong.xyz/gtdmixlqgl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtdmuqxope.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtbhdmjlhd.html

SELECT TRIM(name) FROM users;
来源：http://hz.9152youxi.cn/gtmgpnlohm.html

[Q85] 数值取整
来源：http://hz.xylfe.cn/gtqkjexxwo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.svipenyu.cn/gtklmpvgnh.html

[Q86] 读取 JSON 字段
来源：http://hz.ivvv.top/gtjvxzrano.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtqwqyhupy.html

[Q87] JSON 字段做条件
来源：http://hz.wangdashe.top/gtuydjwvtz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.snrcjt.cn/gtplawcxxa.html

[Q88] 行转列（条件聚合）
来源：http://hz.sufxvd.cn/gtcisvmrhc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.bjfxy.top/gtnlnxmxsk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtgifyefwu.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtbqrkjzlu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gtslqjcwaf.html

[Q90] 生成序号列
来源：http://hz.zhiwuduotai.top/gtmknxhtmk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtramxxbsf.html

================================================================================
来源：http://hz.bjfxy.top/gtrrfwuwue.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gtitqmitpp.html

================================================================================
来源：http://hz.svipenyu.cn/gtsvikuiwa.html

[R01] shebang 与严格模式
来源：http://hz.gaohongyu789.top/gttacstoqo.html

#!/usr/bin/env bash
来源：http://hz.9152youxi.cn/gtzequsgwb.html

set -euo pipefail
来源：http://hz.svipenyu.cn/gtzbztfgih.html

[R02] 变量赋值与使用
来源：http://hz.meibo888.top/gtpeqsnvyp.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtyutoeegm.html

[R03] 只读变量
来源：http://hz.jinqigfzy.top/gtqhhsegzv.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtzwcwcogu.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtthliykkv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtawumcfqa.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gtzlarnwme.html

name="${1:-default}"
来源：http://hz.xuetiantiany.cn/gtzioumvuj.html

[R06] 判断命令是否存在
来源：http://hz.hnqzz.top/gtyunzqooo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jiagoushi.top/gtdivuusdb.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtclacuxmv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gtpvjkfdhl.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtebnlhpip.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenlongwang.top/gtyoneuaww.html

[R09] 字符串比较
来源：http://hz.yj20258888.top/gtutniohqj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhongyouzk.top/gtwokiyfnx.html

[R10] 正则匹配
来源：http://hz.shanyushiyangkeji.top/gtkqvwnuyk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtnfcuqhcr.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtvmntrdca.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtcotyivlr.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangtech.top/gtotlzkkxc.html

stop)  echo "停止" ;;
来源：http://hz.cheryme.top/gtzkobtbhq.html

*)     echo "未知命令" ;;
来源：http://hz.svipenyu.cn/gthkrgnden.html

esac
来源：http://hz.hfpthk.cn/gtganynovr.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gtkjsxiyal.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aibaodan.cn/gtafcvjocv.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtiwsneqye.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtrgxdrodn.html

[R14] C 风格 for
来源：http://hz.andypj.xyz/gthczjyszq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ybcxt.top/gtwzyhhroo.html

[R15] while 逐行读文件
来源：http://hz.xinyue.icu/gtvgxhuxnz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtrjaicjvk.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtfqyiqwzy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtrikikujf.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtvsvsjoer.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtllemwgri.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtaldhelli.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gthuctwpdl.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtgbmjeqvf.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtsnevmume.html

[R20] 关联数组（字典）
来源：http://hz.feifeiyinyue.top/gthakdxvcq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.iojbl.cn/gtkvqdzopc.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtkqdhycoy.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtpxunjika.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtgwiyxiqw.html

echo "${s:0:5}"
来源：http://hz.zhaomingkeji.xyz/gtmsulzenw.html

[R23] 字符串替换
来源：http://hz.yj20258888.top/gtcezakogt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtstkkceyj.html

[R24] 大小写转换
来源：http://hz.wangdashe.top/gtyddniind.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtzoaduwiw.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuanzx.com/gtcrjfzrop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtblbiupll.html

[R26] 命令替换
来源：http://hz.ppjwa.cn/gtyuhtwwka.html

now=$(date +%F); echo "$now"
来源：http://hz.sysykeji.top/gtrfqfsuom.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtvenuymku.html

echo $((1 + 2 * 3))
来源：http://hz.zhijiandao.cn/gtdcbalbvx.html

[R28] 浮点运算
来源：http://hz.feifeiyinyue.top/gtspnwkpjw.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtktxaalel.html

[R29] 定义函数
来源：http://hz.feifeiyinyue.top/gtwzjjuowx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.smart0.xyz/gthjzkucky.html

[R30] 函数返回状态码
来源：http://hz.jiagoushi.top/gtdhlphwhh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtrzrdswzg.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtsfdyijsw.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtlhggojyj.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtnlnbjrhm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtupiblgxx.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gtpxfojvrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtwlrwrxfe.html

[R34] 退出时清理
来源：http://hz.hfpthk.cn/gtzhqvqjjg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtcmhzhhvm.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtownabclo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtdpbxxxmf.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gteyiuqrgn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gthrewxrhz.html

[R37] 把输出赋给变量
来源：http://hz.tianlin.xyz/gttiopsajd.html

files=$(ls -1)
来源：http://hz.ywan-chungtsiang.top/gtjykhrrwc.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtjgnfclgx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nwbrower.top/gtfdivpuro.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtinykrgja.html

cmd > out.log 2>&1
来源：http://hz.xingfuxueyuan.xyz/gtoyvbvsjz.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtnvxuhogo.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtuvuvpizb.html

[R41] 丢弃输出
来源：http://hz.cheryme.top/gtykcfyruq.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtxbsvauut.html

[R42] 输入重定向
来源：http://hz.aibaodan.cn/gtbjnnajrg.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtxcrixtzg.html

[R43] 按名字查找文件
来源：http://hz.aizwys.cn/gtawnuiqie.html

find . -name "*.log" -type f
来源：http://hz.gaohongyu789.top/gthbypoqtm.html

[R44] 按修改时间查找
来源：http://hz.pycfn.com/gttdvzweml.html

find . -mtime -7 -type f
来源：http://hz.snrcjt.cn/gtimaalhwu.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtwospfbqp.html

find . -name "*.tmp" -delete
来源：http://hz.feifeiyinyue.top/gthywrvzqq.html

[R46] 递归替换文件内容
来源：http://hz.tian-w.cn/gtkqstkghn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gtaeqpmaol.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gtdekigfsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gtajourzdu.html

[R48] awk 取指定列
来源：http://hz.sufxvd.cn/gtatpguavk.html

awk '{print $1, $3}' a.txt
来源：http://hz.tianlin.xyz/gtgtpnsrqd.html

[R49] awk 带条件
来源：http://hz.havefunace.top/gtonnzsebg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnxiangtu.top/gtoucjiahr.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtldkbfxbc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtxwhefhph.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtmyfyolud.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtztjyvnqd.html

[R52] 统计行数
来源：http://hz.guowangkeji.top/gtzxvwyqyy.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtafkpucmi.html

[R53] 查看文件头与实时尾
来源：http://hz.zhoulong.xyz/gtmkyovwye.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nwbrower.top/gtyiutzktr.html

[R54] 比较两个文件
来源：http://hz.aibaodan.cn/gtsuwcwgii.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtpmifdwzq.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtblomyett.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtldmhwche.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtddkqxjvj.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gtytdnhtcq.html

[R57] 远程执行命令
来源：http://hz.feifeiyinyue.top/gtkyxqritq.html

ssh user@host 'uptime'
来源：http://hz.guowangkeji.top/gteeeudjoq.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtozvmggex.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.feifeiyinyue.top/gtzhpudafu.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtdfrjipud.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ppjwa.cn/gtqizdxqlh.html

[R60] 只看 HTTP 状态码
来源：http://hz.yonumen.top/gtomfkzbft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtqwulkimv.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtmatheatw.html

df -h;  du -sh *
来源：http://hz.svipenyu.cn/gtckofaevt.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtcdayjypy.html

du -ah . | sort -rh | head -10
来源：http://hz.aizwys.cn/gtfhayfais.html

[R63] 内存与进程
来源：http://hz.sxryk.cn/gtjflylytt.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtcxpslrps.html

[R64] 结束进程
来源：http://hz.nwbrower.top/gtgxukvlcy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtyuqdukwe.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtobmrejor.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhongyouzk.top/gttcruqvgj.html

[R66] 定时任务
来源：http://hz.chenjidiqi.icu/gtmbhkdoba.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtaeirrutb.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gttlajbxzc.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtpbzagwut.html

[R68] 计算文件校验值
来源：http://hz.vqdsnc.cn/gtptdczcjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtmwtajplm.html

[R69] 生成随机密码
来源：http://hz.birdmap.top/gtvakomyti.html

head -c 16 /dev/urandom | base64
来源：http://hz.gaohongyu789.top/gtfxtyilbx.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtrjfowtfs.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gtuymgqmwo.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtqtdjsfrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtlkylvrbz.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtpkqxfcms.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtuqvdkzgq.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gttcfkxrte.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtltrbtjpr.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtotxhowjj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aibaodan.cn/gtkkixflfm.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtbhkfyvqd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtjrvgshse.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtffnfamfe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtcuqstydd.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtjisnteje.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtrxdencfw.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtwlqlugnn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.vqdsnc.cn/gtivjbwfqv.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gtgkvvwhkp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tanke756.top/gttbctyvra.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtnlqgusiz.html

time ./run.sh
来源：http://hz.xingfuxueyuan.xyz/gtqpjawyux.html

================================================================================
来源：http://hz.shuidangran.top/gtzqcuqgzn.html


<!-- 参考信息 -->