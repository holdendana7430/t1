代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.haohaochexian.top/gtxujsrolu.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtoqbalqhl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtvpelbquv.html

[Q31] 分组后过滤
来源：http://hz.svipenyu.cn/gtcodhbucn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenlongwang.top/gtwkpdgtio.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtbmkilxrq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtsckkqail.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtlwoufzxb.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gteoaebeuw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pycfn.com/gtxlauetiy.html

[Q34] 每组取第一条
来源：http://hz.ybcxt.top/gtyqqrmiac.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtkmgagdzk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sweek.top/gtnsvdspwh.html

) t WHERE rn = 1;
来源：http://hz.hnqzz.top/gtzxgnmvgp.html

[Q35] 内连接
来源：http://hz.smart0.xyz/gtmrlrveia.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtbrihfpwp.html

[Q36] 左连接
来源：http://hz.c1oappe.top/gtpqeewupw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtacbctnba.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtuxzddhsj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jyoumei.cn/gtjlzkhozh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.52xcode.cn/gtqpxhnghx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yueranfly.top/gtbgxdwggl.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gttgkkphfo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtmnxennuq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydjk.org.cn/gtfddwszuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xylfe.cn/gtxtihnmif.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gtfirtocpm.html

[Q41] 多表连接
来源：http://hz.ydzc1.top/gtazixvkca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guannengcc.top/gthlvdvctc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pengpengdd.cyou/gtrqxjvduq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hongshengwenyu.top/gtbcrdalas.html

[Q42] 连接条件附加过滤
来源：http://hz.ywan-chungtsiang.top/gtbalndwfh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuanzhike.top/gtneeoozhp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xuetiantiany.cn/gtatqycdbs.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gtqmpyyvkc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gtsmmxqjyl.html

[Q44] IN 子查询
来源：http://hz.shuidangran.top/gtuugpipzw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtsfrbywmy.html

[Q45] EXISTS 判断存在
来源：http://hz.yueranfly.top/gtkqhocnkq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtsugqtfob.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ybcxt.top/gtxeunscxr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gthcmzuxiy.html

[Q47] 与平均值比较
来源：http://hz.fzhhl.top/gtygbmpgme.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtpotbeupp.html

[Q48] CTE 公用表表达式
来源：http://hz.tianlin.xyz/gttrjrcxfm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtvzizpaei.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gthvmcchnz.html

[Q49] 更新单行
来源：http://hz.zhijiandao.cn/gtvwmafzbp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtzgtnmkot.html

[Q50] 批量更新
来源：http://hz.hnxiangtu.top/gtwkoshwki.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ppjwa.cn/gtdsvyyqcm.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtkdagryie.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zycfv.cn/gtxitvltve.html

[Q52] 删除指定行
来源：http://hz.mhx1999.top/gtmzrrbgaz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtxlumoxmz.html

[Q53] 按条件删除
来源：http://hz.hfpthk.cn/gtbgweznxr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.daria6918.cn/gtgofhfoks.html

[Q54] 清空表
来源：http://hz.xuetiantiany.cn/gtdygxuaik.html

TRUNCATE TABLE logs;
来源：http://hz.yvedp.cn/gthsssofnc.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtballspkj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxinkj.top/gtwfmuwldk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nanxuanxn.top/gtxsjeigjj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sysykeji.top/gtxazxdpro.html

[Q57] 行号
来源：http://hz.quarkkingdee.top/gtcxghryxq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangtech.top/gtqqdmtant.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtnoujtoih.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtgzzhwvul.html

[Q59] 分组内累计
来源：http://hz.xuanzx.com/gtvdgxduyp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.c1oappe.top/gtvakbzono.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtmankqoyv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtoyrkntqc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtucikqizu.html

[Q61] 移动平均
来源：http://hz.shzxlz.cn/gtbodkfkgx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aizwys.cn/gtkxrkykgl.html

[Q62] 分组占比
来源：http://hz.sysykeji.top/gttcjfhzex.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtouwpmljv.html

[Q63] 开启事务
来源：http://hz.yj20258.top/gtuzfmoadq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gttrqmhocm.html

[Q64] 提交事务
来源：http://hz.jianghu66.top/gtizumfbbc.html

COMMIT;
来源：http://hz.zhoulong.xyz/gtjkoqmlnr.html

[Q65] 回滚事务
来源：http://hz.hywenlv.cn/gttwfhnraq.html

ROLLBACK;
来源：http://hz.pycfn.com/gtwarttuzl.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gtuliouhfu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtgegjcako.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtnmuskghs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhijiandao.cn/gttqmuvzgn.html

[Q68] 保存点
来源：http://hz.sysykeji.top/gtgrcjqhaw.html

SAVEPOINT sp1;
来源：http://hz.nanxuanxn.top/gtjwmyodum.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtowacyllx.html

[Q69] 查看执行计划
来源：http://hz.meibo888.top/gtxozzereb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.meibo888.top/gtyyjfzaqk.html

[Q70] 更新统计信息
来源：http://hz.ywan-chungtsiang.top/gttcmacfte.html

ANALYZE TABLE users;
来源：http://hz.andypj.xyz/gthysewmer.html

[Q71] 查看建表语句
来源：http://hz.yanxiufei.cn/gtistptotw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtzgkjszhn.html

[Q72] 查看索引
来源：http://hz.fengsongda.top/gtsambklmo.html

SHOW INDEX FROM users;
来源：http://hz.ydzc1.top/gtycmoonwf.html

[Q73] 查看表状态
来源：http://hz.cheryme.top/gtistsqvxa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.quarkkingdee.top/gtwccibbrs.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtxdqckbcj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtsbcyosba.html

[Q75] 日期格式化
来源：http://hz.zhoulong.xyz/gtfnkwprfi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jiagoushi.top/gtnoduuvlp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtdnydyxms.html

[Q76] 按天统计
来源：http://hz.vqdsnc.cn/gttmciraqx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinghuilouyu.cn/gtjmxddzen.html

[Q77] 时间加减
来源：http://hz.gzhubu.top/gtlzmnzuoy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtgihlgiob.html

[Q78] 当前时间
来源：http://hz.snrcjt.cn/gtnqpzxepo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhengqikj.top/gtbjckkecy.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gtgbuqfith.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtxcyjvqej.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtbadcvjgr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sxryk.cn/gtqnqvzdbv.html

[Q81] 字符串替换
来源：http://hz.zhengqikj.top/gtbefulujo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtjqhthprd.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtxrfmlyxd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aizwys.cn/gtxqbggkfb.html

[Q83] 大小写转换
来源：http://hz.chenjidiqi.icu/gtjuexduer.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtjolplbcs.html

[Q84] 去除首尾空格
来源：http://hz.jianghu66.top/gtuawdxrnr.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtdethppeu.html

[Q85] 数值取整
来源：http://hz.zhoulong.xyz/gthumhqnpm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gzhubu.top/gthyhubzzs.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtjkiymwhg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gttmymcdmz.html

[Q87] JSON 字段做条件
来源：http://hz.hnxiangtu.top/gttdyuuwug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtukrvfnpo.html

[Q88] 行转列（条件聚合）
来源：http://hz.shzxlz.cn/gtzwjlojhb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xziqi.cn/gtptpzwtxn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtkuaxrffr.html

[Q89] 判断表是否存在
来源：http://hz.xingfuxueyuan.xyz/gtfearwmru.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhiwuduotai.top/gtybwtqkrf.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtlqvvgaln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhiwuduotai.top/gtnltpkdds.html

================================================================================
来源：http://hz.sufxvd.cn/gtorgoeqvj.html

R. Bash 专题
来源：http://hz.yj20258.top/gtdemzeykv.html

================================================================================
来源：http://hz.cashguo.top/gtugnghijv.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gttfdmhffd.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtibgffdlh.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtjkkuzulh.html

[R02] 变量赋值与使用
来源：http://hz.jianghu66.top/gturmpdhrb.html

name="Tom"; echo "$name"
来源：http://hz.nanxuanxn.top/gtfzkptjjn.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtpgncigux.html

readonly PI=3.14
来源：http://hz.zhijiandao.cn/gtzugwatww.html

[R04] 位置参数
来源：http://hz.guannengcc.top/gtpwcgbhnh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gtptqqwgaf.html

[R05] 参数默认值
来源：http://hz.aizwys.cn/gtkcvhqpvd.html

name="${1:-default}"
来源：http://hz.xylfe.cn/gtqdbxuvxt.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gturujxqzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gttgjdqoxl.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtwrabotyi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gthrsmhduq.html

[R08] 数值比较
来源：http://hz.yvedp.cn/gtbfseybxs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xinyue.icu/gtiqrkompn.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtffnojokh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258888.top/gtffudgufs.html

[R10] 正则匹配
来源：http://hz.iojbl.cn/gtfmgejrlt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gthfkypkbz.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gtpqacpnak.html

case "$1" in
来源：http://hz.tanke756.top/gtspxwvezw.html

start) echo "启动" ;;
来源：http://hz.xziqi.cn/gtuldfcjut.html

stop)  echo "停止" ;;
来源：http://hz.zycfv.cn/gtlkjxjnda.html

*)     echo "未知命令" ;;
来源：http://hz.zdqjudy.top/gtpbjkscyq.html

esac
来源：http://hz.bjfxy.top/gtoxmxxtgc.html

[R12] for 遍历文件
来源：http://hz.zhiwuduotai.top/gtvdthaqxw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtcqjguqcf.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gteglokbyl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gtvmeblaku.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtpugcwjvn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtembhnycr.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtdrhmhvji.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shzxlz.cn/gtnuqsaiko.html

[R16] until 等待条件
来源：http://hz.ivvv.top/gtwsqqxtda.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gtpdioyyij.html

[R17] 数组定义与取值
来源：http://hz.cashguo.top/gtczcjrubn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ehwqpu.com/gtdqvwisfy.html

[R18] 遍历数组
来源：http://hz.jiagoushi.top/gtjzvbqnuo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xylfe.cn/gteyfduiec.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtgjyrnnmr.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtdbykttdw.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtsomdtcqy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxinkj.top/gtppdyzrmg.html

[R21] 字符串长度
来源：http://hz.shanyushiyangkeji.top/gteptgirva.html

echo "${#s}"
来源：http://hz.dashuyun.cn/gttsmajqbn.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtipfgkkte.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtfcrsxufw.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtrfgfeqhe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtzlbwiayz.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtpdoizptl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gtliiiwddk.html

[R25] 去后缀 / 去前缀
来源：http://hz.shuidangran.top/gtfmyexuna.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258888.top/gtwcyurlud.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtmutdzoyj.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gtdedwldgk.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtxjacybsk.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtlbuxzznx.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtkvdluqhl.html

echo "scale=2; 10/3" | bc
来源：http://hz.sxryk.cn/gtlalfzouj.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtqehvaqul.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gteunubhpq.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtvcsumalr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jianghu66.top/gtgffvspbc.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gtzptybzym.html

f() { local x=1; echo "$x"; }
来源：http://hz.svipenyu.cn/gtcytgkiux.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gtpnkgvvao.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.andypj.xyz/gtgwnjmidn.html

[R33] 捕获错误并提示行号
来源：http://hz.dashuyun.cn/gtofzbqnit.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dianchejie.cn/gtnnsjfcvq.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtuuahtnej.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gtcnyxsogt.html

[R35] 后台执行并等待
来源：http://hz.svipenyu.cn/gtkeptojjk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.havefunace.top/gtciylvwkk.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtypyzrpix.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gttkqvhnve.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gttdzsvxvm.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtbmralcub.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtknitrazp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gteuotvzji.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtybmwjbvw.html

cmd > out.log 2>&1
来源：http://hz.fengsongda.top/gtqqztbffb.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtxwsqltmt.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gttflvkwtg.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtghotficq.html

cmd >/dev/null 2>&1
来源：http://hz.yanxiufei.cn/gtjnofdcmy.html

[R42] 输入重定向
来源：http://hz.zhoulong.xyz/gthqesueac.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtwcmtihzx.html

[R43] 按名字查找文件
来源：http://hz.chenlongwang.top/gtczhmfijq.html

find . -name "*.log" -type f
来源：http://hz.cucudq.cn/gtcjkeypra.html

[R44] 按修改时间查找
来源：http://hz.jinqigufen.top/gtaprdedfe.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtarjjhauz.html

[R45] 批量删除
来源：http://hz.zdqjudy.top/gtqtwcnevg.html

find . -name "*.tmp" -delete
来源：http://hz.shzxlz.cn/gtiuphcpuy.html

[R46] 递归替换文件内容
来源：http://hz.dianchejie.cn/gtlggozjfe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtnrxvoolr.html

[R47] sed 单行替换
来源：http://hz.birdmap.top/gtvxakjptk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.c1oappe.top/gtyhdnlbgu.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtisrmwbtf.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinghuilouyu.cn/gtxajnaltb.html

[R49] awk 带条件
来源：http://hz.ehwqpu.com/gtdhikcdej.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtjwdasrlj.html

[R50] awk 求和
来源：http://hz.gzhubu.top/gtwxaecyec.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yanxiufei.cn/gtdxfgtmza.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtpzhrnpan.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.smart0.xyz/gtbcaagcml.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtwzhmchna.html

wc -l a.txt
来源：http://hz.cashguo.top/gthdmzxrvo.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtupuqlwbe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tanke756.top/gttulydzte.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtdkheedux.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gthfctuwch.html

[R55] 压缩与解压
来源：http://hz.tianlin.xyz/gtqwtxywia.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtoggixqfi.html

[R56] 远程拷贝
来源：http://hz.shuidangran.top/gtnsorczcv.html

scp file user@host:/path/
来源：http://hz.aibaodan.cn/gtuntyitrf.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtdvpcunxf.html

ssh user@host 'uptime'
来源：http://hz.hnqzz.top/gtjltdkxzh.html

[R58] 下载文件
来源：http://hz.nanxinkj.top/gtefqnmqaw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtfaqmynhe.html

[R59] 发 POST JSON
来源：http://hz.yvedp.cn/gtyuelahsy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtlxblitfv.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gtgmgifbdd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtdmhaiakx.html

[R61] 磁盘占用
来源：http://hz.cqqwz.cn/gtntuzqemy.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtuaoixhgv.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gtjcwybcbw.html

du -ah . | sort -rh | head -10
来源：http://hz.mhx1999.top/gtpqjlezxm.html

[R63] 内存与进程
来源：http://hz.zhengqikj.top/gthpvulwdr.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gtccqvlpap.html

[R64] 结束进程
来源：http://hz.kuanghao11.cn/gtzolqgufd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnxiangtu.top/gtsxganshd.html

[R65] 查看端口占用
来源：http://hz.jlsjyb.cn/gtymediloi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtiftfotpu.html

[R66] 定时任务
来源：http://hz.guannengcc.top/gttfvhwrsb.html

crontab -e;  crontab -l
来源：http://hz.sufxvd.cn/gtosntownd.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtrovocqee.html

openssl rand -hex 16
来源：http://hz.jianghu66.top/gtssesefhr.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gtmokwhmfy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtxphrontr.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gtoterbqng.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gttvbwtohj.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtytpqsghp.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtvqkbdlno.html

[R71] 日期格式化
来源：http://hz.nanxuanxn.top/gtqktyuxyl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinyuanbaomall.cn/gtiknfazxa.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtkwfeoucf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtxssvjmlo.html

[R73] 分割大日志
来源：http://hz.kuanghao11.cn/gtxaceigwp.html

split -l 1000 big.log part_
来源：http://hz.guannengcc.top/gtqexmgodf.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtkhmewlxm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gttgityjte.html

[R75] 导出环境变量
来源：http://hz.jiagoushi.top/gtbpzrxhvo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gtxqpjdqqz.html

[R76] 使用临时文件
来源：http://hz.smart0.xyz/gtcdrveiaf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtzrkbupjm.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtsmkppwjb.html

read -rp "请输入: " ans
来源：http://hz.dashuyun.cn/gtnfojuvlu.html

[R78] 交互式菜单
来源：http://hz.cheryme.top/gtnueawfvv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtrazxnqto.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtdmfoamvs.html


<!-- 参考信息 -->