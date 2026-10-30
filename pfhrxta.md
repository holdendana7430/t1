代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggcxwstyu.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gyouhbrnl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdknuasx.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgqilsry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlqsazek.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhdwbhjl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gohddsrpn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxavlfrya.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gmlopukjq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gedctqnix.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhdexdwp.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubxlukzw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvavfwvzp.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxlfdac.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxytajjcc.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdxzxoti.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryvodbef.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/guibfogrl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxxmfukj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganowjoto.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gkbcqoczf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvbfoty.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkmfecxf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryfbpkqb.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpckkrnrd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqebbgmq.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gublbrgni.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gkeixkeps.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gehoxquhm.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhvenytv.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gcgvkuokc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeubyhpx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/greuetmak.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gouargosl.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaqweqbc.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqwwzplb.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbfxwplbk.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpxrxzos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gpgcmwrbm.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gvefyjgdr.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gazjkspoz.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gildbtbur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewgffhky.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gmccowjib.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqreqant.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/ghubqvqlo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gybuyfuvl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gputyszpb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gflcuxnod.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gswyoevqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpfodsxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gcsmoffqq.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ggbrqhmgb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzwfxtrf.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gtjgjjhfi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/goqhtbbuh.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsdjugeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gmeimsrua.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbtiyibh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gyopifgwl.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqkqioad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gezmneabz.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkbfpeci.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaysgois.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/goouhqkpo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuzagiar.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllgspjtv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyomyidbr.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqzvnua.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkgxqeqh.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gbpjgowlr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guutatnhg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gcemxpaop.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkyovpef.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqedidbch.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgpfmhum.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/ggvprkkra.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwibsvsag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjsczwum.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gllaqntzs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhtbwaat.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtpdmbym.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gakwyurgd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqtbvnwyp.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtfppsnys.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqsmolmwt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/guozecdat.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gwanvvupt.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gofpduftj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgggxqdb.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gnzarvrxb.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbwwhva.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gorczrizg.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoptjbvx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gqyvktjck.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/giifskkwh.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnyquywtq.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpkazhhpq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjeolkjv.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfypkclwg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaaqtpyy.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/guuzqupts.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ggrvoftpa.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmbomcua.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/guygakads.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghocbwyao.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gufqyglsq.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gavsbukrl.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/goiuvdhoe.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gkuhcxizf.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gdlkkvysy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gjiyihfcc.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikdewuhc.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnwpuhxpz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkagznekj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmpequtux.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhgqtize.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gkhybeyqt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbzukuvoh.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gurastrvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyfzpojfh.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gccsupmnz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvzhhczy.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gsochedrh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbnvszcf.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gryzqfapy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqwwmpnm.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcmyfubrh.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grxffwvmm.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gsnomrotc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkuaihrp.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtwbzufs.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzwvvrfvw.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gaiooatqa.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqakydlks.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsvywxgto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdylsrjec.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyjgirrf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcjotdkp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhidtzqf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwouogxya.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbjmqowqc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaszctcga.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpalcdsw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsmljncw.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbghawwok.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxkzkng.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdxratjot.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyxhthyws.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gkmckaoyr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gofvgcvgj.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwcwhqua.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnclttycf.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gqxlhctbd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtroepmbh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gbczkgpwu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gjwxqhtra.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiutqomf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gnxlodlnq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gdunlpleh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwmgegkf.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtvjkpxyy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkttytidm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gauisjoeb.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqillncy.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gszcnjjas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gyzryyitz.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gbupuibni.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gedxlfswp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpcpxmdf.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gnlwzczwu.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gvzwykrqi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gjdnwnsuj.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gyytxmwfk.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbawivlcr.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsntkgvl.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwxazapgc.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqzklefzj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnlunvox.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gdkuoxggc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gihaxnngh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhrwpqkj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvywopvu.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxckhafxh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtxresas.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfvieryu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzqbxcju.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsyppbln.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbukiswh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gscvnwryq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gygmrygwz.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gdepzmafj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/giefwbcfk.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdkktyjyl.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxelkeynn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gflztcwky.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtdgvvrv.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsjrakzmz.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/govresist.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gvhhpcrrk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbgrrlaa.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gprdqnhdk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkjzwktv.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaycbiyo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvshwpger.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghznuvnjq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gdcrofylv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlfczguk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmdqzpqdi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkblekibb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gyysgszgk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjdxxxzw.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gjxtklaze.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzfsgxure.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gwjtblrem.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveehgixl.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gytmldtqe.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfotrrgrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gtrjltjxp.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwsrrtmi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfspmeqb.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/girceeqlq.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gksyxsyjq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyxhehxk.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkbplrco.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrykenwu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyogibow.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gfgivjree.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwltaemd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gwelmubea.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ghadunmqz.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghccdhodt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gstoskmjy.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvzgeqab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/guzuakmdi.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfpjbhnms.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gtfdyrkmk.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gkugzcolv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gabmadhaq.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gklnguinb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhyelurn.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gutfabdbo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdenjomw.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvrwkvfq.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gblwyxrrg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzebguyz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gomompbum.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdywjnab.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtsmqzzp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gscocdsii.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrwdymrn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gigbbpdfe.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/grrvuqxgs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcifdhzyj.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoosoztm.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqnlqhnc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfypuggl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvcthbhb.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/ghipefvqs.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/glfcycaso.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gipnoqsry.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gjyaaymmh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/ggrmebdpu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gikohwtkz.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaziseony.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/glfhwjxjx.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gowvnueng.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glnmkwxfp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gadmhrqhd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gddtijcds.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvrmbcyb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcawzqmba.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gbhlznnkf.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqwsbft.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwespllge.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxvfqncc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gqwroxlao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grsmsdamk.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ggontlvqd.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grbknsboy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gocyyvfgl.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyisnjzh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqljznwxr.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gulltcyvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkibrzysy.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvsbqlld.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgoprszt.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvwyasmn.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjgdhqimh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ghiiehuzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwegzxf.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfuixhqni.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/glorrvkfe.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gebzntkll.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/giumgwlst.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrupznm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshmxkupk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchdznoul.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gljasoynr.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiguqpoa.sHtML


<!-- 参考信息 -->