代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gtkrgwzbzn.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtyhtreubm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtsgxbuujd.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtbylhsiva.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.fengsongda.top/gtzbyhsnfs.html

[Q32] 分组拼接字符串
来源：http://hz.kuanghao11.cn/gtakxcolis.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtrewlyjyd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhixingplan.top/gtlbyzkdcl.html

[Q33] 多列分组
来源：http://hz.ydjk.org.cn/gtefboddfv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shangyingyoupin.top/gtdptpwzsu.html

[Q34] 每组取第一条
来源：http://hz.svipenyu.cn/gtgixuvknp.html

SELECT * FROM (
来源：http://hz.dianchejie.cn/gtmrxxqxba.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinyuanbaomall.cn/gthxejkpdt.html

) t WHERE rn = 1;
来源：http://hz.wangshuangyany.cn/gtxhfugpjv.html

[Q35] 内连接
来源：http://hz.ppjwa.cn/gtfnzlmykk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtifxshxxa.html

[Q36] 左连接
来源：http://hz.nanxinkj.top/gtzdpkwfjd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gteujliucb.html

[Q37] 右连接
来源：http://hz.jinghuilouyu.cn/gtgxgznmos.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxuanxn.top/gtohhdretl.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtdmmlhpmt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtiaelfwxx.html

[Q39] 自连接（查上下级）
来源：http://hz.ppjwa.cn/gtexjwhafx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gtdqogdvkp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.iojbl.cn/gthxkmdqmf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.bjfxy.top/gtzojkkqob.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangdashe.top/gtnjdvcsve.html

[Q41] 多表连接
来源：http://hz.andypj.xyz/gtzykidkpy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.meibo888.top/gtrravybpt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tian-w.cn/gtbsupqhie.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtumtiedpw.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtubbvbisp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gtxkbysgfr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guannengcc.top/gtomjgqliy.html

[Q43] 标量子查询
来源：http://hz.shzxlz.cn/gthyyowywg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daria6918.cn/gtkyzdhkjm.html

[Q44] IN 子查询
来源：http://hz.sweek.top/gtlkpqocsr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtriupfshj.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtbqiaivpx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tian-w.cn/gtkmpxpqpw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtdyvsjjek.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xinyue.icu/gtegnajhcz.html

[Q47] 与平均值比较
来源：http://hz.sweek.top/gtdqfqmvnc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtgpxwbmwr.html

[Q48] CTE 公用表表达式
来源：http://hz.zhiwuduotai.top/gtzbwnbbov.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jlsjyb.cn/gtqjixqpoa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hammf.cn/gtvrowzdtx.html

[Q49] 更新单行
来源：http://hz.bjfxy.top/gtqkycamcp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtfrkllxvf.html

[Q50] 批量更新
来源：http://hz.andypj.xyz/gtotbwizba.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shangyingyoupin.top/gtkoxpdtnp.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtgfbaatla.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gttsnpilwl.html

[Q52] 删除指定行
来源：http://hz.yj20258.top/gtrnggcaku.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tanke756.top/gtxjdoncmw.html

[Q53] 按条件删除
来源：http://hz.jinghuilouyu.cn/gtcrcezsqu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxinkj.top/gtnvkubird.html

[Q54] 清空表
来源：http://hz.cheryme.top/gthumynnwx.html

TRUNCATE TABLE logs;
来源：http://hz.hnqzz.top/gtbcgqystw.html

[Q55] 排名（并列占位）
来源：http://hz.ppjwa.cn/gtuhhrvrlu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xziqi.cn/gtxcwktcju.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cucudq.cn/gtyrcgvbaw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.cheryme.top/gtatlfawwg.html

[Q57] 行号
来源：http://hz.feifeiyinyue.top/gthkcjpoiw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxuanxn.top/gtecqyecom.html

[Q58] 累计求和
来源：http://hz.chenzaomai.com/gtfhjmpenb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tian-w.cn/gtxfcwtxrz.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtmormjvqo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtxzqfjqsq.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhengqikj.top/gtoxceevgz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtktwpzgbb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtqatggpfq.html

[Q61] 移动平均
来源：http://hz.gaohongyu789.top/gtvupvvhsh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtozmfkzyj.html

[Q62] 分组占比
来源：http://hz.fzhhl.top/gtdmmqvxle.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtuubcmaqx.html

[Q63] 开启事务
来源：http://hz.zhijiandao.cn/gtbvaeyeyl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhoulong.xyz/gtemlxhuzj.html

[Q64] 提交事务
来源：http://hz.tian-w.cn/gtwkxuvydc.html

COMMIT;
来源：http://hz.chenlongwang.top/gtgowbiryp.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gttjvcilfe.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtkaivogxo.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangtech.top/gtgooiinlw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gtvbdqigol.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtdcdyvuhj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.kuanghao11.cn/gtdpzbggxg.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtmtrgjpoj.html

SAVEPOINT sp1;
来源：http://hz.snrcjt.cn/gtrwfshxag.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtnuugmxih.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtxkyniaqd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangshuangyany.cn/gtquvbabsx.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtgjyqeyld.html

ANALYZE TABLE users;
来源：http://hz.yj202588.top/gtlkaetkno.html

[Q71] 查看建表语句
来源：http://hz.sxryk.cn/gtimqpleqb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gtnnmqieiv.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtmmfovfvu.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtlhenksau.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtmocibobu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtoetjtqcq.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtghmomddk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtqopppoaj.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gtqjximdje.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gthspykefz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.andypj.xyz/gtgqslhvkc.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtzmcfxjbb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtfyrrpank.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gtdvunkfyq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtgggroycx.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtcmnffaoq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtxbftfnab.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtremnazlp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cashguo.top/gtgckhxzpa.html

[Q80] 字符串截取
来源：http://hz.dashuyun.cn/gtsrserltj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gotoacloud.top/gtnfrqsava.html

[Q81] 字符串替换
来源：http://hz.yuxming.cn/gtuduhokiv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gtyumnuqqz.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtbldeapcg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shuidangran.top/gtfdezscfj.html

[Q83] 大小写转换
来源：http://hz.9152youxi.cn/gtbxpyhafz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.mhx1999.top/gtyhpxwvwc.html

[Q84] 去除首尾空格
来源：http://hz.chenjidiqi.icu/gtuilkomug.html

SELECT TRIM(name) FROM users;
来源：http://hz.c1oappe.top/gthklieegy.html

[Q85] 数值取整
来源：http://hz.gotoacloud.top/gtjhkjhusw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.vqdsnc.cn/gtongjcbne.html

[Q86] 读取 JSON 字段
来源：http://hz.haohaochexian.top/gtwrvyysyp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtayqewqya.html

[Q87] JSON 字段做条件
来源：http://hz.xingfuxueyuan.xyz/gtzajhlpbu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gtgivxtrxw.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gtcfnodjxj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hysaishi.cn/gthmajyzav.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gtwpacjhhj.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtfqfwendt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtseagsdqx.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gtvylcynoj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtzsuoigoq.html

================================================================================
来源：http://hz.cqqwz.cn/gtqcnhoffa.html

R. Bash 专题
来源：http://hz.shanyushiyangtech.top/gtmdsglach.html

================================================================================
来源：http://hz.sysykeji.top/gtbvodibjx.html

[R01] shebang 与严格模式
来源：http://hz.shangyingyoupin.top/gtxbjgwomy.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtctqynlvf.html

set -euo pipefail
来源：http://hz.zdqjudy.top/gtzmtivftt.html

[R02] 变量赋值与使用
来源：http://hz.daxiang520.top/gttjqkrjrq.html

name="Tom"; echo "$name"
来源：http://hz.yueranfly.top/gtqoolhzzj.html

[R03] 只读变量
来源：http://hz.sufxvd.cn/gtiyzyasll.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtmtvcwebx.html

[R04] 位置参数
来源：http://hz.sweek.top/gthagtnkeh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sufxvd.cn/gtvjjkamsu.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtmsladhez.html

name="${1:-default}"
来源：http://hz.yanxiufei.cn/gtrnfhgxof.html

[R06] 判断命令是否存在
来源：http://hz.guowangkeji.top/gtpvzvurts.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.kuanghao11.cn/gtloxzjjgf.html

[R07] if 判断文件
来源：http://hz.cashguo.top/gtbieytdnz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxuanxn.top/gtiisyetls.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gtgtickhpn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yvedp.cn/gtfrofwkte.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gtqzhdhbiu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jyoumei.cn/gtpcwofuzy.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gttbgmgqcm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.meibo888.top/gtyyanslgn.html

[R11] case 多分支
来源：http://hz.shanyushiyangtech.top/gtohgkzpyp.html

case "$1" in
来源：http://hz.snrcjt.cn/gtbdujqrtw.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gtgxkxadax.html

stop)  echo "停止" ;;
来源：http://hz.yj202588.top/gtmtrugfyy.html

*)     echo "未知命令" ;;
来源：http://hz.zycfv.cn/gtdqguhuut.html

esac
来源：http://hz.zhixingplan.top/gtvpfvbyau.html

[R12] for 遍历文件
来源：http://hz.xingfuxueyuan.xyz/gtswbekztn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gtogpqtvws.html

[R13] for 计数循环
来源：http://hz.yueranfly.top/gtvnakgndd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xylfe.cn/gtqapluzsb.html

[R14] C 风格 for
来源：http://hz.zhixingplan.top/gtbqiemezy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtduouajwr.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gthhvlnybq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtkusmbasw.html

[R16] until 等待条件
来源：http://hz.zhoulong.xyz/gtywjdgrlo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtwvkbmxgw.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtandcmila.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tanke756.top/gtukpyncyi.html

[R18] 遍历数组
来源：http://hz.hongshengwenyu.top/gtaaiddffc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aibaodan.cn/gtekjxnsks.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtghcseyoc.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtjwzchodo.html

[R20] 关联数组（字典）
来源：http://hz.nanxinkj.top/gtidoaiuza.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtzdkkjmpv.html

[R21] 字符串长度
来源：http://hz.ivvv.top/gtnbixqeiz.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtmklluueh.html

[R22] 截取子串
来源：http://hz.chenlongwang.top/gtsvqqceon.html

echo "${s:0:5}"
来源：http://hz.jinqigfzy.top/gtnqvnmams.html

[R23] 字符串替换
来源：http://hz.wangdashe.top/gtegjmcpxr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gtnhcubjco.html

[R24] 大小写转换
来源：http://hz.hongshengwenyu.top/gtdqliihbm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sweek.top/gthpalprxc.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtbzmalszy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.redwolf501.top/gtdazgysel.html

[R26] 命令替换
来源：http://hz.wangshuangyany.cn/gtnduxbkrn.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtkyvzbdpd.html

[R27] 算术展开
来源：http://hz.gaohongyu789.top/gtbnqbsamt.html

echo $((1 + 2 * 3))
来源：http://hz.52xcode.cn/gtaokqnygp.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtapjqcegl.html

echo "scale=2; 10/3" | bc
来源：http://hz.aizwys.cn/gteerjhmnd.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtefjfdukd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtxwyfmhgm.html

[R30] 函数返回状态码
来源：http://hz.aibaodan.cn/gthrmkacua.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigfzy.top/gtibmdhvrn.html

[R31] 局部变量
来源：http://hz.wangshuangyany.cn/gtihpglhlt.html

f() { local x=1; echo "$x"; }
来源：http://hz.jiagoushi.top/gtkdbwssuf.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtdrtlyoep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtsfbkqmrz.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtqbkjimag.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.bjfxy.top/gtmfmmljkh.html

[R34] 退出时清理
来源：http://hz.chenzaomai.com/gtuwsvggde.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtajbfgpbd.html

[R35] 后台执行并等待
来源：http://hz.52xcode.cn/gtfrbrosqc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.0kj1m.cn/gtlytmyffl.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtmlgjvugu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtjnjmnzhx.html

[R37] 把输出赋给变量
来源：http://hz.sysykeji.top/gtbhhlvnqv.html

files=$(ls -1)
来源：http://hz.yongpay.top/gtmpyovazj.html

[R38] 管道串联
来源：http://hz.hammf.cn/gtlddqixsn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtxopxjiih.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtewcymhhv.html

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gtzrztecxg.html

[R40] 追加写日志
来源：http://hz.aizwys.cn/gttktvbrrq.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gthsppvmyw.html

[R41] 丢弃输出
来源：http://hz.zhaomingkeji.xyz/gthqczbxaj.html

cmd >/dev/null 2>&1
来源：http://hz.redwolf501.top/gtuzxmjrca.html

[R42] 输入重定向
来源：http://hz.dianchejie.cn/gtnwpucocu.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gtwldxrqat.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtjadclyir.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtqntwwfnf.html

[R44] 按修改时间查找
来源：http://hz.yj202588.top/gtedkhvkiq.html

find . -mtime -7 -type f
来源：http://hz.xziqi.cn/gtnpevpbvb.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gtyfhhtqwp.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gtzycdvmcu.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtnjuenkml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtdmihnbjm.html

[R47] sed 单行替换
来源：http://hz.ehwqpu.com/gtpqmmlbxl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gtisufrgkd.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtpaonbcyh.html

awk '{print $1, $3}' a.txt
来源：http://hz.ydjk.org.cn/gtplfxrvnu.html

[R49] awk 带条件
来源：http://hz.daria6918.cn/gtwuxboaos.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtidqyafnu.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtzuvgyxcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.smart0.xyz/gtyufzttzl.html

[R51] 排序去重取前几
来源：http://hz.52xcode.cn/gtsujyjggi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daxiang520.top/gtaxxgjaeu.html

[R52] 统计行数
来源：http://hz.yonumen.top/gtdwffghua.html

wc -l a.txt
来源：http://hz.feifeiyinyue.top/gteilzlurv.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtmjtzvshe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtpsmsohlf.html

[R54] 比较两个文件
来源：http://hz.0kj1m.cn/gtctyxmcts.html

diff a.txt b.txt
来源：http://hz.52xcode.cn/gttysliylu.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtltxqlhmr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gtqltbcxep.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtjmehppwf.html

scp file user@host:/path/
来源：http://hz.meibo888.top/gtqzhlovxn.html

[R57] 远程执行命令
来源：http://hz.cheryme.top/gtubzzcvfr.html

ssh user@host 'uptime'
来源：http://hz.cdnleiting.top/gtevmeuebg.html

[R58] 下载文件
来源：http://hz.fzhhl.top/gtdtpscdxu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangshuangyany.cn/gtuyaicrwj.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtryxwnjam.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtmhsmtpwh.html

[R60] 只看 HTTP 状态码
来源：http://hz.52xcode.cn/gtchqlzvts.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangtech.top/gtvxqbdari.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtmbrlutft.html

df -h;  du -sh *
来源：http://hz.pengpengdd.cyou/gtqkmvlchl.html

[R62] 找最占空间的文件
来源：http://hz.dashuyun.cn/gtkzxfxisx.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gtrhsruksp.html

[R63] 内存与进程
来源：http://hz.aibaodan.cn/gtkzidkdep.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gtrgyflbwz.html

[R64] 结束进程
来源：http://hz.pycfn.com/gttzjmnjrw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtupyrevub.html

[R65] 查看端口占用
来源：http://hz.cheryme.top/gtfplpdfcg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gtsrhbguyf.html

[R66] 定时任务
来源：http://hz.quarkkingdee.top/gtpyxsxjkj.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtkambotsv.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtxvfzofsh.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtjvbnedxu.html

[R68] 计算文件校验值
来源：http://hz.shuidangran.top/gtslujsneu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtjpmhngyy.html

[R69] 生成随机密码
来源：http://hz.yj202588.top/gtgcqxaiju.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtfdewviok.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gthpgvwcre.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtlvdxpnok.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtevhutvre.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtcvdbonuw.html

[R72] 等待端口就绪
来源：http://hz.0kj1m.cn/gtqostygvs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gogol.net.cn/gthykfkwph.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtzyjxktri.html

split -l 1000 big.log part_
来源：http://hz.tian-w.cn/gtziyulmrw.html

[R74] 批量重命名
来源：http://hz.haohaochexian.top/gtvlfiowih.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daxiang520.top/gtjgwkbivu.html

[R75] 导出环境变量
来源：http://hz.andypj.xyz/gtwtdatgcn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gtngmdzcwj.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gtifkooyap.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtwamtrqmt.html

[R77] 读取用户输入
来源：http://hz.redwolf501.top/gtymtntxtk.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtjflqwabx.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtqswmblru.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.iojbl.cn/gtfgwgzajj.html

[R79] 解析命令行选项
来源：http://hz.yj20258.top/gtxwyygpzp.html


<!-- 参考信息 -->