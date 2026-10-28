代发 wailian999

[Q36] 左连接
来源：http://hz.birdmap.top/gtvsptxycc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtslzishmm.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtrvydancx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtlyvgblbm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnxiangtu.top/gtzrtcoxxb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gttrjdbbvu.html

[Q39] 自连接（查上下级）
来源：http://hz.ybcxt.top/gtinwqnzha.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gotoacloud.top/gtsyidrxec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gtywqlghno.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtcdtqybks.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtkatuktjg.html

[Q41] 多表连接
来源：http://hz.meibo888.top/gtkfratjpq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtxlnrllju.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ehwqpu.com/gttjkzokye.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gtcxasimbm.html

[Q42] 连接条件附加过滤
来源：http://hz.daxiang520.top/gtbiexsigd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.snrcjt.cn/gtpoxznpuh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gtjillpetp.html

[Q43] 标量子查询
来源：http://hz.cucudq.cn/gtkogvfkrp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dashuyun.cn/gtkbpsnifp.html

[Q44] IN 子查询
来源：http://hz.shuidangran.top/gtbbcnyijj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.bjfxy.top/gtrpbppurn.html

[Q45] EXISTS 判断存在
来源：http://hz.yueranfly.top/gtwsvrkrks.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtxlftviwe.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtyqljnscp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtejzpnreq.html

[Q47] 与平均值比较
来源：http://hz.hysaishi.cn/gthwzxpdlj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangshuangyany.cn/gtsqsjhvya.html

[Q48] CTE 公用表表达式
来源：http://hz.zhiwuduotai.top/gtlhmraehg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yuanzhike.top/gtqqsglvzv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tanke756.top/gtpcwkivac.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtoeuvnlhz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hongshengwenyu.top/gtufareggf.html

[Q50] 批量更新
来源：http://hz.zhoulong.xyz/gtnbdvkkwt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuanzx.com/gtxncccjga.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gthqbbtdnp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.tanke756.top/gtjailiwzk.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtewhnceij.html

DELETE FROM users WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtroojasoz.html

[Q53] 按条件删除
来源：http://hz.xuetiantiany.cn/gtoipafkpa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtoglrmknd.html

[Q54] 清空表
来源：http://hz.dashuyun.cn/gtabtziphp.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtzqmiqvta.html

[Q55] 排名（并列占位）
来源：http://hz.jyoumei.cn/gtjvybthpg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtsjlsyshq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gtomaozrjh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gtleawvxts.html

[Q57] 行号
来源：http://hz.bjfxy.top/gttcczbgbv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtcvlnttde.html

[Q58] 累计求和
来源：http://hz.hongshengwenyu.top/gtaqgpiliq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gtufvtvyed.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtmmdovrep.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtkrjlrgvj.html

[Q60] 取上一行 / 下一行
来源：http://hz.cqqwz.cn/gtvlbqbiuw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtxycyjyqi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.snrcjt.cn/gteattdmye.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtewcxihbn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtlvktgvot.html

[Q62] 分组占比
来源：http://hz.hfpthk.cn/gtsvoqyhwn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtzzzthbfc.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gtqcamblti.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fzhhl.top/gtknyijtll.html

[Q64] 提交事务
来源：http://hz.hongshengwenyu.top/gtfygufqcq.html

COMMIT;
来源：http://hz.yvedp.cn/gtefzpyiaj.html

[Q65] 回滚事务
来源：http://hz.daxiang520.top/gtznebqmik.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtwmnguprm.html

[Q66] 行锁查询
来源：http://hz.jinyuanbaomall.cn/gtsjvxkdrg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhongyouzk.top/gtvftmvnxj.html

[Q67] 设置隔离级别
来源：http://hz.jqgfzy.top/gtucqrxetg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhoulong.xyz/gttsnsczvp.html

[Q68] 保存点
来源：http://hz.iojbl.cn/gttzbhwkbm.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtctnhyjsp.html

ROLLBACK TO sp1;
来源：http://hz.gaohongyu789.top/gtgdcbtosb.html

[Q69] 查看执行计划
来源：http://hz.meibo888.top/gthvmlnilp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangdashe.top/gtddvmxmxp.html

[Q70] 更新统计信息
来源：http://hz.birdmap.top/gtidjvrzlh.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtbvwbills.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtvuazrovr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtkymmxqso.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtygusjskm.html

SHOW INDEX FROM users;
来源：http://hz.quarkkingdee.top/gtlsqfzbge.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtmzhmqpag.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gogol.net.cn/gtyzmsafwi.html

[Q74] 强制使用索引
来源：http://hz.chenzaomai.com/gtezgbcpsy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.fzhhl.top/gtlphyzgqz.html

[Q75] 日期格式化
来源：http://hz.nanxuanxn.top/gtbzcvletc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtxikfcxbl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtniquqyxc.html

[Q76] 按天统计
来源：http://hz.yvedp.cn/gtumtrjbnw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtypgbfawl.html

[Q77] 时间加减
来源：http://hz.ydjk.org.cn/gtasfjtzal.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xingfuxueyuan.xyz/gtxdzbpwto.html

[Q78] 当前时间
来源：http://hz.tianlin.xyz/gtgwoxcfjl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ppjwa.cn/gtlioqcnua.html

[Q79] 字符串拼接
来源：http://hz.tian-w.cn/gtwesugcau.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtzgndwdun.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gthwmmecbk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.pengpengdd.cyou/gtbactjntp.html

[Q81] 字符串替换
来源：http://hz.gzhubu.top/gtggeyojgw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ybcxt.top/gtmakxrygz.html

[Q82] 字符长度与字节长度
来源：http://hz.redwolf501.top/gtovnaddpg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuxming.cn/gtlvkezfka.html

[Q83] 大小写转换
来源：http://hz.yvedp.cn/gtswgrukcy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jlsjyb.cn/gtbrqojesn.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gthrgjnmnm.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtueudxwvq.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtumlywlji.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtnlakdzus.html

[Q86] 读取 JSON 字段
来源：http://hz.birdmap.top/gtudhypxvy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gtztwlaovq.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtiuqqcics.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtndypdcfd.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxuanxn.top/gtpgszzndd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guowangkeji.top/gtqgauvqap.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tanke756.top/gtjuoknvnn.html

[Q89] 判断表是否存在
来源：http://hz.pengpengdd.cyou/gtiowcrkgr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gttjmfugle.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gtswjdaciv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtnnwramkx.html

================================================================================
来源：http://hz.zycfv.cn/gtxxjtvaeh.html

R. Bash 专题
来源：http://hz.yongpay.top/gthiwptwag.html

================================================================================
来源：http://hz.ehwqpu.com/gtgczlwswg.html

[R01] shebang 与严格模式
来源：http://hz.tanke756.top/gtiivnqoyy.html

#!/usr/bin/env bash
来源：http://hz.yuanzhike.top/gtrmvlfqhj.html

set -euo pipefail
来源：http://hz.dashuyun.cn/gtonbhgfgl.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gthrsugdgc.html

name="Tom"; echo "$name"
来源：http://hz.iojbl.cn/gtxfklzieh.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gtptroaqru.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gttlwstgfh.html

[R04] 位置参数
来源：http://hz.guannengcc.top/gtgfygmnkt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sysykeji.top/gtodtggdnq.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gthumqosks.html

name="${1:-default}"
来源：http://hz.c1oappe.top/gtxpumetfl.html

[R06] 判断命令是否存在
来源：http://hz.svipenyu.cn/gthjdlfcgx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jlsjyb.cn/gtegeroyna.html

[R07] if 判断文件
来源：http://hz.yj20258.top/gtvihczhws.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.bjfxy.top/gteyietsnf.html

[R08] 数值比较
来源：http://hz.xuetiantiany.cn/gtyvpershi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zdqjudy.top/gtixzzftnl.html

[R09] 字符串比较
来源：http://hz.feifeiyinyue.top/gtmfazfftn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shuidangran.top/gtavowpjsi.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtaspuihjc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ywan-chungtsiang.top/gtabimwyky.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gtvcgroefr.html

case "$1" in
来源：http://hz.cdnleiting.top/gtyitssmxk.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtzrrughnw.html

stop)  echo "停止" ;;
来源：http://hz.nanxinkj.top/gtnfiuxpqn.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtodfyzjeh.html

esac
来源：http://hz.ydjk.org.cn/gtshmuwueq.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gtpbwdnssg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hongshengwenyu.top/gtkiczlntw.html

[R13] for 计数循环
来源：http://hz.wangdashe.top/gthnatebho.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sysykeji.top/gttpfthuvw.html

[R14] C 风格 for
来源：http://hz.tianlin.xyz/gthzeljejx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gttkjafcdg.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gteolhwkgy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gtvlbanaoc.html

[R16] until 等待条件
来源：http://hz.yangfankeji.com/gtrjtmitjw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtcyzdvhmt.html

[R17] 数组定义与取值
来源：http://hz.yvedp.cn/gtqbhdvtoe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.birdmap.top/gtbfujcbhr.html

[R18] 遍历数组
来源：http://hz.cashguo.top/gthizuaybh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pengpengdd.cyou/gtjffxddel.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtkbazmohh.html

echo "${#arr[@]}"
来源：http://hz.xziqi.cn/gtagudwqxp.html

[R20] 关联数组（字典）
来源：http://hz.chenlongwang.top/gtzorseizo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydjk.org.cn/gtnitbxmek.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtkswkszyr.html

echo "${#s}"
来源：http://hz.hongshengwenyu.top/gtzzlaplhh.html

[R22] 截取子串
来源：http://hz.cheryme.top/gtobcdpkyh.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gthtyovfzl.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtuurrcfqh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtgyyndkow.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtwthxuujh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cashguo.top/gtdxavxkwr.html

[R25] 去后缀 / 去前缀
来源：http://hz.smart0.xyz/gtoyzonjcj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.316326.xyz/gteqdsudnr.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtihjwsqcy.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtxrmyefiz.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtznkslhpz.html

echo $((1 + 2 * 3))
来源：http://hz.shangyingyoupin.top/gtdamnlefu.html

[R28] 浮点运算
来源：http://hz.sufxvd.cn/gtaejlekby.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtktjhghwh.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtkhotzezd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pycfn.com/gtjcewwrnr.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gtaeozldcw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guannengcc.top/gtbvuyupaf.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtimhejkze.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtryvdnzev.html

[R32] 参数个数校验
来源：http://hz.pengpengdd.cyou/gtgwelzocc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtpzyvgpav.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gteyhdqtym.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtpezlewat.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtcqilwxgs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtypsctfyh.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtopufqxng.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuxming.cn/gtzsxpdmhx.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtebozhewy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtadgskeew.html

[R37] 把输出赋给变量
来源：http://hz.jiagoushi.top/gtnekcyyah.html

files=$(ls -1)
来源：http://hz.pengpengdd.cyou/gtwjqasvbl.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gthvneifls.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtnvsfpezz.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigfzy.top/gtztyxwjrm.html

cmd > out.log 2>&1
来源：http://hz.52xcode.cn/gtgqlvwxqg.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtevmyqnsu.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtkcposqwg.html

[R41] 丢弃输出
来源：http://hz.jqgfzy.top/gtqmsfizky.html

cmd >/dev/null 2>&1
来源：http://hz.sweek.top/gtjlzbibly.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gtnjfxcgdv.html

wc -l < a.txt
来源：http://hz.jiagoushi.top/gtljtolrmv.html

[R43] 按名字查找文件
来源：http://hz.cucudq.cn/gtmphjdjjs.html

find . -name "*.log" -type f
来源：http://hz.jinghuilouyu.cn/gtgqvirrvr.html

[R44] 按修改时间查找
来源：http://hz.cqqwz.cn/gturcztjmf.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtowmxunny.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtbquezmvd.html

find . -name "*.tmp" -delete
来源：http://hz.zhoulong.xyz/gtyciicabc.html

[R46] 递归替换文件内容
来源：http://hz.andypj.xyz/gtpnxzxlqz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtewjlajfw.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtnghrydwj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shuidangran.top/gtepwiuqml.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gttudhkgqr.html

awk '{print $1, $3}' a.txt
来源：http://hz.dashuyun.cn/gtjosqnvmi.html

[R49] awk 带条件
来源：http://hz.jinqigfzy.top/gtwhmktzrd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gtgksdledi.html

[R50] awk 求和
来源：http://hz.hammf.cn/gtcnmcmuuy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hfpthk.cn/gtigvzqibl.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtepxnnmql.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shuidangran.top/gtlzefqydu.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtqrlgaikc.html

wc -l a.txt
来源：http://hz.316326.xyz/gtvhaykwgc.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gtdnanpadq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtijqvfsam.html

[R54] 比较两个文件
来源：http://hz.shangyingyoupin.top/gtdgrvhnsh.html

diff a.txt b.txt
来源：http://hz.wangshuangyany.cn/gtycobjuey.html

[R55] 压缩与解压
来源：http://hz.zdqjudy.top/gtdsuznpxd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.quarkkingdee.top/gtynzglrll.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtrxgsakvn.html

scp file user@host:/path/
来源：http://hz.tanke756.top/gtbycffthr.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gtycutxxmc.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtknymcabq.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtkvzzuweq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gtcywzvopj.html

[R59] 发 POST JSON
来源：http://hz.fengsongda.top/gtyhxleczu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gtjaaayynb.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtqtttsawu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtatnxzgsy.html

[R61] 磁盘占用
来源：http://hz.cashguo.top/gtjwegycql.html

df -h;  du -sh *
来源：http://hz.daria6918.cn/gtsnjfrwju.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtojfcthvt.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtnismzxpe.html

[R63] 内存与进程
来源：http://hz.iojbl.cn/gtdxgbrwng.html

free -h;  ps aux | grep nginx
来源：http://hz.xylfe.cn/gthjvwyjjq.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gtvhvyiskd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cucudq.cn/gtoseqkpzf.html

[R65] 查看端口占用
来源：http://hz.tanke756.top/gtbaesvxqc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtdyaktcbt.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtshtuwiix.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtgljllapi.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtgziafcjv.html

openssl rand -hex 16
来源：http://hz.hfpthk.cn/gtfyaoyoff.html

[R68] 计算文件校验值
来源：http://hz.gaohongyu789.top/gtgbumwdtd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtxouwkdzc.html

[R69] 生成随机密码
来源：http://hz.fzhhl.top/gtiedqnqjs.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgfzy.top/gtxecbxits.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gtuscigaez.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtegslxqku.html

[R71] 日期格式化
来源：http://hz.xziqi.cn/gtddwosjeq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtnhqfcttk.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtsqgvncnu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtasgjsnfv.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtriupptbz.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtkjenxcjf.html

[R74] 批量重命名
来源：http://hz.yonumen.top/gtcsdlirfw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtyafzaudc.html

[R75] 导出环境变量
来源：http://hz.zycfv.cn/gtzcjbpwdl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtqcuwissw.html

[R76] 使用临时文件
来源：http://hz.nwbrower.top/gtxcphpnbw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtgxqxlgdh.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gttumjfuga.html

read -rp "请输入: " ans
来源：http://hz.yangfankeji.com/gtfezvmphu.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtirfzvesa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtwmlcdkgn.html

[R79] 解析命令行选项
来源：http://hz.zdqjudy.top/gtxmadjghb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtmdhjaukj.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtmrtgithh.html

time ./run.sh
来源：http://hz.yuxming.cn/gtnocqicxf.html

================================================================================
来源：http://hz.shzxlz.cn/gtfnfqkkjx.html

S. C / C++ 专题
来源：http://hz.chenzaomai.com/gtpnzhkkzb.html

================================================================================
来源：http://hz.cheryme.top/gtrturbvsa.html

[S01] C：Hello World
来源：http://hz.zhixingplan.top/gtgcsfyzno.html

#include <stdio.h>
来源：http://hz.jqgfzy.top/gteppjrblc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pycfn.com/gtskrbpfsp.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gtezonswzt.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtamjlhtnp.html

[S03] C：读入整数
来源：http://hz.hnqzz.top/gttvnxcazr.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtwxcaeqpz.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtleyktfqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuxming.cn/gtudmrqcqp.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtuyagtonf.html


<!-- 参考信息 -->