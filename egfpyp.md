代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gtlfezckdm.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtjiwgidqx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtojfigrxt.html

[Q31] 分组后过滤
来源：http://hz.cdnleiting.top/gtuzuzlesp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.meibo888.top/gtnmcxmdkg.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtuuqfwhjy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtjdpyirzf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxuanxn.top/gtogxvlrlk.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtvnanswgw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yueranfly.top/gtnermniae.html

[Q34] 每组取第一条
来源：http://hz.vqdsnc.cn/gtspkajumy.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtdodpdhfm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhongyouzk.top/gtwgimdwwj.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtatyrcyap.html

[Q35] 内连接
来源：http://hz.feifeiyinyue.top/gtiggepjyf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtlqcfvuzy.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtnkneevby.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtjqezyuri.html

[Q37] 右连接
来源：http://hz.ywan-chungtsiang.top/gtkflbtarb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtdhzjfqee.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xylfe.cn/gtqdpiscph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sysykeji.top/gtqsuouhgs.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gtpjprtjwd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gtgqtmqwjr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.dashuyun.cn/gtvatynpnb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.kuanghao11.cn/gtoktrgydk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hongshengwenyu.top/gtyvzuxqbd.html

[Q41] 多表连接
来源：http://hz.ywan-chungtsiang.top/gtgacystxk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ivvv.top/gthfzhfnce.html

JOIN users u ON u.id = o.user_id
来源：http://hz.52xcode.cn/gthajfepzz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258888.top/gtjmflvuij.html

[Q42] 连接条件附加过滤
来源：http://hz.sweek.top/gthbaoelkf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yuxming.cn/gtkcxjqxjd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuxming.cn/gtjcurmldf.html

[Q43] 标量子查询
来源：http://hz.sweek.top/gtzdejjtiy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtyasqlzvk.html

[Q44] IN 子查询
来源：http://hz.xingfuxueyuan.xyz/gtrprtepbx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gteutykqsh.html

[Q45] EXISTS 判断存在
来源：http://hz.xuanzx.com/gtrwybjhei.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtdhxhiitq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtbxjadhgy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gttcesjxre.html

[Q47] 与平均值比较
来源：http://hz.mhx1999.top/gtbmlkicvr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.svipenyu.cn/gteyibsqac.html

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gtrccdhwaq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gturchszei.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jianghu66.top/gttpjdrmpd.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gthroqiohh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtmxiwurdu.html

[Q50] 批量更新
来源：http://hz.sufxvd.cn/gtloqrbsdt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtelutztsr.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gtgvitfhuf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtfgjnylfa.html

[Q52] 删除指定行
来源：http://hz.daxiang520.top/gtuujibsgi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.316326.xyz/gtuiyvudve.html

[Q53] 按条件删除
来源：http://hz.jlsjyb.cn/gtymcicaul.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtuxxvbjjy.html

[Q54] 清空表
来源：http://hz.zhongyouzk.top/gtslhkzxxa.html

TRUNCATE TABLE logs;
来源：http://hz.pengpengdd.cyou/gtnwzmgyby.html

[Q55] 排名（并列占位）
来源：http://hz.snrcjt.cn/gtauiplyma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtuiiamifo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtiwtvfrft.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtojkdizny.html

[Q57] 行号
来源：http://hz.dianchejie.cn/gtciztsiij.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xziqi.cn/gtabaqvyzy.html

[Q58] 累计求和
来源：http://hz.zhixingplan.top/gtlwpqwoyv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fzhhl.top/gtcptdotzy.html

[Q59] 分组内累计
来源：http://hz.jinghuilouyu.cn/gtgghgirjy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtfcpjyssl.html

[Q60] 取上一行 / 下一行
来源：http://hz.fzhhl.top/gtwuywyufy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtgbogbtpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.birdmap.top/gthcmfzddk.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtlvmpvtrs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtayszetyv.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtybyqhvgv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtfthvqldl.html

[Q63] 开启事务
来源：http://hz.aibaodan.cn/gtlnpgusws.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.vqdsnc.cn/gtuzzkdnmr.html

[Q64] 提交事务
来源：http://hz.shangyingyoupin.top/gtkqldaodk.html

COMMIT;
来源：http://hz.yonumen.top/gtghebcifz.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtvtkubwgh.html

ROLLBACK;
来源：http://hz.cashguo.top/gtqrcunlvy.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangkeji.top/gtvistfxih.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.mhx1999.top/gtoigychia.html

[Q67] 设置隔离级别
来源：http://hz.zhongyouzk.top/gtbbwxlegz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.svipenyu.cn/gtdegygqzh.html

[Q68] 保存点
来源：http://hz.pengpengdd.cyou/gtfvgwxreu.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtmbgdeqdm.html

ROLLBACK TO sp1;
来源：http://hz.ivvv.top/gthvjginuq.html

[Q69] 查看执行计划
来源：http://hz.gotoacloud.top/gtkttkraei.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtfjzbgrnc.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gtrhwfhizc.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtufzuzznr.html

[Q71] 查看建表语句
来源：http://hz.ydjk.org.cn/gtmqiroaiw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gtbnacsutw.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtfpmqiswg.html

SHOW INDEX FROM users;
来源：http://hz.cdnleiting.top/gtronnvwcj.html

[Q73] 查看表状态
来源：http://hz.tian-w.cn/gtttjielpx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.smart0.xyz/gtpnaqffsz.html

[Q74] 强制使用索引
来源：http://hz.ppjwa.cn/gtbhquvwrl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.kuanghao11.cn/gtinltkhkp.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtqrzsbpmp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtwgwttcev.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgufenzy.top/gtwyblohqw.html

[Q76] 按天统计
来源：http://hz.yueranfly.top/gtfvkfnkrp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtemrvtubb.html

[Q77] 时间加减
来源：http://hz.daria6918.cn/gtqfneuxxw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gzhubu.top/gtznlkzlhr.html

[Q78] 当前时间
来源：http://hz.zhijiandao.cn/gtcedptute.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtfruyksho.html

[Q79] 字符串拼接
来源：http://hz.zhoulong.xyz/gtttcycybh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhiwuduotai.top/gtzxkzkdaq.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gtfxuqpoxe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvdvikzkf.html

[Q81] 字符串替换
来源：http://hz.hongshengwenyu.top/gteubsfqah.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gthwwmzbph.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gtctvimkyi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtnkqlrgnd.html

[Q83] 大小写转换
来源：http://hz.quarkkingdee.top/gtqrcrrgkm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yanxiufei.cn/gtmvpdkrpy.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtgyzjzstw.html

SELECT TRIM(name) FROM users;
来源：http://hz.9152youxi.cn/gtvmkaucbz.html

[Q85] 数值取整
来源：http://hz.jinyuanbaomall.cn/gtzxaiasfi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sufxvd.cn/gtrmdfogfz.html

[Q86] 读取 JSON 字段
来源：http://hz.shangyingyoupin.top/gtsqkqbnym.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtxwbokkdk.html

[Q87] JSON 字段做条件
来源：http://hz.jlsjyb.cn/gthhnybtbi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenjidiqi.icu/gtzjooysgm.html

[Q88] 行转列（条件聚合）
来源：http://hz.yonumen.top/gtapxwdwjp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtvgskuunu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtgzndmxjv.html

[Q89] 判断表是否存在
来源：http://hz.zhongyouzk.top/gtpjqwjojb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yuxming.cn/gtmisndgnv.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangtech.top/gtsoxfmeiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtmofoymob.html

================================================================================
来源：http://hz.316326.xyz/gtdopkqvdy.html

R. Bash 专题
来源：http://hz.shanyushiyangkeji.top/gtydfauhxe.html

================================================================================
来源：http://hz.yvedp.cn/gtiqxtqeof.html

[R01] shebang 与严格模式
来源：http://hz.hywenlv.cn/gtaqyicrex.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtojshmqmu.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtampfnwok.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gtsepabqno.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtzjuwgrlx.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtbisfxhke.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gtevzswgxq.html

[R04] 位置参数
来源：http://hz.ivvv.top/gtcqjziavb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnxiangtu.top/gtmwwyybbh.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtidumhjxm.html

name="${1:-default}"
来源：http://hz.jyoumei.cn/gtxmtgsszj.html

[R06] 判断命令是否存在
来源：http://hz.shuidangran.top/gtdoeejkoz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtxphmgsoz.html

[R07] if 判断文件
来源：http://hz.tianlin.xyz/gtsrsbwyte.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gtuahqwqkp.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtstwcjyuz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tian-w.cn/gtpejezjxe.html

[R09] 字符串比较
来源：http://hz.hnqzz.top/gtpveyrsno.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtdpzgxlzc.html

[R10] 正则匹配
来源：http://hz.tanke756.top/gtjxpljuba.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ywan-chungtsiang.top/gthjderhto.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtpotvpgoq.html

case "$1" in
来源：http://hz.mhx1999.top/gtyhwisynq.html

start) echo "启动" ;;
来源：http://hz.ppjwa.cn/gtbreuouie.html

stop)  echo "停止" ;;
来源：http://hz.feifeiyinyue.top/gtrveadwrp.html

*)     echo "未知命令" ;;
来源：http://hz.dianchejie.cn/gtqbafxwnx.html

esac
来源：http://hz.ivvv.top/gtgycuqvgd.html

[R12] for 遍历文件
来源：http://hz.ehwqpu.com/gtklfmqlld.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtcknvhimy.html

[R13] for 计数循环
来源：http://hz.aibaodan.cn/gtoxvatmic.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtjrpfoawt.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtodixpqxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yonumen.top/gtnofltods.html

[R15] while 逐行读文件
来源：http://hz.guowangkeji.top/gtlueiprer.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtsnmguzkn.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtjpgfjoxo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.iojbl.cn/gtififzhjw.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtdobxjxsn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtmjgxyxyr.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtrfqjffct.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtvnwvnbcl.html

[R19] 数组长度
来源：http://hz.havefunace.top/gtxgledzat.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtgdebaadi.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gtdpiagzmc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jqgfzy.top/gtsrxzpwii.html

[R21] 字符串长度
来源：http://hz.jinqigfzy.top/gtfpnukpvd.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtlcvqfzkh.html

[R22] 截取子串
来源：http://hz.ybcxt.top/gtorhjoazs.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtbbydhxhq.html

[R23] 字符串替换
来源：http://hz.yangfankeji.com/gtqlklsqya.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hywenlv.cn/gtbxhndonu.html

[R24] 大小写转换
来源：http://hz.hnqzz.top/gtbgoeakgn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jiagoushi.top/gtjbwzyfko.html

[R25] 去后缀 / 去前缀
来源：http://hz.c1oappe.top/gtgictunxq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtawjsehqh.html

[R26] 命令替换
来源：http://hz.guannengcc.top/gtrvfqnkmp.html

now=$(date +%F); echo "$now"
来源：http://hz.feifeiyinyue.top/gtsvusevek.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtixykdaxf.html

echo $((1 + 2 * 3))
来源：http://hz.dashuyun.cn/gtjqkggqid.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtjmlzvohm.html

echo "scale=2; 10/3" | bc
来源：http://hz.sufxvd.cn/gtpgrjiukn.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gtjrzhjjoe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnxiangtu.top/gtlisgzqfy.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtorghtnfv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gtqcnbjdfj.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtofqcgnws.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxinkj.top/gtiujbfvnr.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtwfobuzld.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtvegqzjbp.html

[R33] 捕获错误并提示行号
来源：http://hz.svipenyu.cn/gtgorlivbf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sweek.top/gtlcooirqf.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtnlkqzxka.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtefgwakng.html

[R35] 后台执行并等待
来源：http://hz.jianghu66.top/gtiprmqfmd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cashguo.top/gtfbhakwhb.html

[R36] 并发执行多个任务
来源：http://hz.zhijiandao.cn/gteerwiezn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtuhsdndah.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtbylspipc.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtukdrjwjx.html

[R38] 管道串联
来源：http://hz.nanxuanxn.top/gtxfrcdqdp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtzbpjeldt.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtxfmikqjw.html

cmd > out.log 2>&1
来源：http://hz.cucudq.cn/gtsaylsbxr.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtpacrhiyu.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtolukryvg.html

[R41] 丢弃输出
来源：http://hz.xylfe.cn/gtkxmgijfb.html

cmd >/dev/null 2>&1
来源：http://hz.feifeiyinyue.top/gtegmcssse.html

[R42] 输入重定向
来源：http://hz.sxryk.cn/gtnrttmkel.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtacuwavhp.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtusvjuwvb.html

find . -name "*.log" -type f
来源：http://hz.gzhubu.top/gtcxrcwgyy.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gttauhjunm.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtvvabfozx.html

[R45] 批量删除
来源：http://hz.yuxming.cn/gtzikyrcfh.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtnspbldxn.html

[R46] 递归替换文件内容
来源：http://hz.jinqigufen.top/gtbwfogxut.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtaohzxjsl.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtqfgbbkhl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtnkbqvmqm.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtolqcafpa.html

awk '{print $1, $3}' a.txt
来源：http://hz.jyoumei.cn/gtucsjlzba.html

[R49] awk 带条件
来源：http://hz.jlsjyb.cn/gteaatwkhw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtnamksqze.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtuggwiwkn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gtsqkwljuj.html

[R51] 排序去重取前几
来源：http://hz.yangfankeji.com/gtnlotxpbi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sweek.top/gtmkdqacet.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtmnbmfeku.html

wc -l a.txt
来源：http://hz.yongpay.top/gtluyasazz.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtkdxfulua.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gtepuhtewt.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtwbyltyyi.html

diff a.txt b.txt
来源：http://hz.cheryme.top/gtpowicqnt.html

[R55] 压缩与解压
来源：http://hz.zdqjudy.top/gtezgonxwk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtzaxbzwzs.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtgugborhd.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtpfxrxmjw.html

[R57] 远程执行命令
来源：http://hz.fzhhl.top/gtvnmmcorl.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gtxldpziwy.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtwzkrlebr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gtjelovvnf.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gthdsjgasa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtzavdqkrd.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtmyznjjmy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cdnleiting.top/gttphzricx.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtybwhccfh.html

df -h;  du -sh *
来源：http://hz.yuxming.cn/gttnwaqmdn.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtqxnhrqlm.html

du -ah . | sort -rh | head -10
来源：http://hz.snrcjt.cn/gthuvffbff.html

[R63] 内存与进程
来源：http://hz.kuanghao11.cn/gtinslkski.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtalhrfnhm.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtkngeefjk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydzc1.top/gtjegdbfhh.html

[R65] 查看端口占用
来源：http://hz.gaohongyu789.top/gtxtzyexas.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtyojkbtpm.html

[R66] 定时任务
来源：http://hz.jiagoushi.top/gtxrxomuyd.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gtcipczgct.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtnsvsjrvf.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gtuipmjuxx.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtcjattqnc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fengsongda.top/gtpxtvntta.html

[R69] 生成随机密码
来源：http://hz.sufxvd.cn/gtakllqidw.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtsbeebqsm.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtcrpityjm.html

date +%s;  date -d @1700000000
来源：http://hz.sysykeji.top/gtuabylgwf.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtfkyzowqe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtiqtlrgyg.html

[R72] 等待端口就绪
来源：http://hz.wangshuangyany.cn/gtipyueolf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtbezipujn.html

[R73] 分割大日志
来源：http://hz.xinyue.icu/gtwfiqoekd.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtqusmjuqw.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gthqpekwkw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gtwgqitycl.html

[R75] 导出环境变量
来源：http://hz.jinqigufen.top/gtszacyiki.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtyapmyedz.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtdzamhrkm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtrgbdaqtw.html

[R77] 读取用户输入
来源：http://hz.jinqigufen.top/gtftinckte.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtjchsjhhz.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtjbchwnlv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.bjfxy.top/gtihpvkqwi.html

[R79] 解析命令行选项
来源：http://hz.jinqigufen.top/gtcvetyfyf.html


<!-- 参考信息 -->