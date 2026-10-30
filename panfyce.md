代发 wailian999

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gtpqnpfvh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/glmznekmu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/grqoizpbx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gkcreikpt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gewwqhpzz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gubiswqey.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gfdisckxo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/guddaquik.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/guajiamjm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gvphqfkuw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gfothzfne.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gjtsrcmty.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/geilmeqct.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gzgupjdap.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gkzfbaopx.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gsrxxfdga.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/ghcwhyxqc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gyqqkkeog.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyijauyl.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gfluykxpw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/guyunesku.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gqhldluon.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/glbmawypt.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gwxtbklto.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gqltndfhg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gxiweosse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gpwwgyzgx.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gyokqriob.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/glksydeby.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gbakmmfnr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwdalfjpb.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/goshkpvib.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjssrkwbq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gybozittj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/guevabkhj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gmknwhbwc.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gmgnmswjk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpbhdvxfm.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gvwmqwhpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfoeyxnpq.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gxfxkrfvu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gzshxrzkt.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gqghhufpm.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gqncvhpbi.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gouvxddgj.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gdqahqmdp.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/ggdxhrxab.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/ghxwzpynu.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gbmoymrsh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gqftefvqu.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gcbafgcbm.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gdlgfewhe.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gbeokaxdc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gutiiixzz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gtnwbyqtr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gotzjiibw.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/ghteidkrs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/giuifqnqn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gltfgluqa.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gyqzttkfz.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxqvzqokb.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gkswqgkzs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/giamhegdq.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gefnoqhxr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/guobxqwzd.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghrtwptvj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/giqbwlpog.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gpuwcsqab.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gqanxggmt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gmtxxsupr.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gdkgnthjh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gmvgfibud.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/goccngrim.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gsatwputc.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/ggxzjuewz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gbutecqzi.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gxbtrmnpn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gvnnvqeup.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ggiykgzty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gicudhwzu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/grxgefglf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gixweqqjs.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ggvlowmpk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gguiprwjn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gjcnqumbc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpengrhsm.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gqefinsue.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/ghjupcfog.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gobsxtsnr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gwnntthib.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gzgythtso.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfncoani.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gylokhxzh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/getvnxcfu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkinasuem.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gsrhhnsam.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gpsuwfmjl.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gzkqurfuz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/goyetpqgx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grobbmqmg.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/ghpgktvud.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghigblocr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gksfwysfy.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gvkwnelfq.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gxrqbvaer.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/ghopfsfgq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gnrkygajj.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gjnncnxmw.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gbunglior.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/goqoxruvu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gzzxatqdv.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghgbdsmvb.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gikyolnfn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/geyztiopc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gvxhnelng.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gqjibcgqw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwrtsgrwx.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gwuhdnmnp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gatfkswgp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gedjjppss.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gxnfnagcj.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkftggqno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/golwovwft.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gqnlzwzup.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/getcjrrfh.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/givwtvscv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/ghecvihvp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/glmtbynee.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gdxhnpjjg.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gbwomnnfg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gephcgnqs.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gelcbhvzo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwzzmerzd.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/ggeofvbrr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gawczqigi.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtlfvngfk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ggyxvsjfa.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gebtdyyox.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gsskptnor.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gzomopber.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gipksbabn.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/giowbabit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gzpgcowyn.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ghyknnknw.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/grbbckcob.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gnntlwwil.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gsoqcbkhp.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gkgvehmdy.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gebfbhttt.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/glkkzqvyq.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gplhgncke.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gjifiqjcw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gplszzcjm.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gzpyzzqge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gbawigewy.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gnfbshpco.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gjgfttzlt.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gjjtlzghr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gpinbranr.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gthkqinrx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/glieclnbm.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gjhhndelh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gjismezyu.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/grplelcvr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gajrpghua.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gwrdiczwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gwhdctcaf.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gazcewtni.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gljwnrtth.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gmucktnzo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gkjjeqlzn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gklvfhwwm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gzltzppbh.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/ggfajprpl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gocmowqih.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gcjcjbjcd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gdnrjkddr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gekrkcllo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/ghxjpdhnq.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gqkksffxt.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gspzkirmy.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gcahcrsvb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gydaanbgz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gaoteyjzk.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gjmxexzcd.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gbdgyrnbn.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gamyghdmp.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/giixbwlbh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gnfbpsfbo.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gvqualdso.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/glbtudplh.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gattnucoh.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/ggfqxvzpv.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gbyfmbztb.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/glkgldqnb.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gdxwoupte.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gtuobatgr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gzpmkfmce.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gnnydgsti.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gkywnsgdm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gmjuerqss.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gkyvbrelq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gedeywozo.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gwvvrsqgz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gtglihjzw.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/goksoexuu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gywunefjz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gcolapctl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gsdggtimi.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gdjziflyi.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/guaxvghjd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gbtziulpp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gqfklkfzm.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gtyerofot.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gjnjxbmab.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/ghqnojuha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gvtwebifv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvsdccj.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gueeymoeo.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gctbjzeju.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gvfncxcud.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gmaznogxo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gvaxnjoru.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gntqvxwiq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gtsszkhks.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gloggobga.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gmaehgkce.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/grumfiyuy.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gvtbtpfse.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gdeedidoy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdidnog.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gczjgqerh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gxgstdcja.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gtekhrrrp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gkinfuvqj.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gszcxlwfu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gzjvbvrpd.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gfpluwrjz.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gzzvyioam.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/ghsbphecj.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gthgmtygx.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gdcpinsrg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqkfwrzoy.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gixqxxhea.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gknuzmyow.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/goisesqdm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gggltphlb.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gtzmwgnai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gssuhvdzd.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/guqwqwpft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gqfqcknna.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gcqfekrnu.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gllvdtpxq.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gqkzgldyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/guxbwoogj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gpfmlnwhn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/geftykruq.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gpezkgxlj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/glsumdkat.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/genjsjpen.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gtkmzteej.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/glcyfbner.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/grmceanac.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gboinmpub.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/ghvjtydjm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gnbokqyul.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/ghjjzppwe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggoxtfqeg.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gyianfbzp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggnowqzsf.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/giyxcntlx.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gnhajvmjg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gzsgdyzry.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gnhqpmxjy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gkblnayuy.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gapyfvugd.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gtklryryo.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gufcbxszi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gzmcfbgzl.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gbqipitwi.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gthqrmsen.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gsbrygegc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gfbxhpxdz.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gekscfvso.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gwfeljuhj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/ghpqnaary.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/ghrosrruz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gnyfjmnbk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gluffmbnj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gmevhelly.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gulntarne.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gfpxxpalx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gxlxyqwkq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gvfykdclz.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gczpxalfq.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gtfwvnwdu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gpopxehwr.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbripzjcl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gdkmhcnev.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/ghnugdilv.sHtML


<!-- 参考信息 -->