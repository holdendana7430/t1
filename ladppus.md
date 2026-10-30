代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/galsdyrxs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsrxdmeh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbbvwdwt.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvhjewpj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gileecvqj.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/grymppjow.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghisevuls.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrmxwmrb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gexbmuvpp.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gosmwynqf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgcstqgv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyofgldju.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gwpnchpos.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmnfomnt.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gaawsmrdu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gumhmalce.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gvmysqsdq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqnaafzt.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoodjvky.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/glcyxuswf.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gifplvxim.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnquooc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsuwtovb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganvpsssm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnysifnnc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvvycgp.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyxqadjk.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/goouzqtku.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqiehtif.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasgjeuya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwtenhon.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/grrjbymdw.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyefhqfhz.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gftlbnsbe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoszyvtp.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkatozncj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkianehl.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/grxmlrpie.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/grbzavpfk.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/golnsprlo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gqnrwjgbv.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggizaktpn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqhyqfofm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gdvjtsxat.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/ghewuinnu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnivdzxl.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/ghquvchmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/glkujtckf.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/grnzkqhmu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gakklkumr.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/guqseuiuz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrodgxqv.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gnthzuhlo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrhhwdtn.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfrqxhtd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gachaqfod.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemvkrhri.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjfnshmwc.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glgeqcxxs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaksumdkf.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvulxibo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gygowwbxe.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/guqdmrodr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylokciwy.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gbtymrlvh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/guncuiwrs.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyzzzaeo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gsaynrfbz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrtkmpvy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmxnwfnr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmkjzifk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjajhdyj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxlqaeay.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcbxaycf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpfojoqj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goskakfmq.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gzfgyqgwn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkhtblywc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrvibexj.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gpedkafxo.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gpudhgoph.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbxwvkd.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gaywfgpnv.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzgjjukwt.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gultxeybx.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggamsqwdd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqgmietm.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkteebzxn.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqqaaagk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvdbuvft.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbuixxfcy.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvosphdgo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghhcdxeft.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glkxhzxpn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxkbefuyy.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guwnnsbqp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghijqeysa.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxwpksiux.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmixalubr.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gxuivoksy.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxqbhlbb.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gcapsrgge.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsahxjwei.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gysvftfks.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gqezzhguc.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcjandl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvtgwgyom.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuqdpanh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghgaakisy.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gubgbdope.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrbdpbif.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsuhoqf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtvszmys.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gufqanury.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtbqbvtg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuuhbysn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gydgysvjs.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gophzxcmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glupuelqq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gipgdpdpp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/genhyfzul.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gxofburzn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbncwvkvk.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gyomkvgml.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glwkqzsub.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gffkuhbzc.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbgysimw.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqbdqrsz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwektxbhk.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxltuuxip.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gykddghlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/goyysnetp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfnmqzps.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkvammcr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbinficq.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtjgqcsu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gtuxbeidg.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxuuqrxj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gugaxnozr.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzuvtsoxw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grionsmru.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbbcntjzs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gzkidmeaw.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmnwevizr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzkzhzbiv.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gyndgfbmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gotmvejxp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbblyfyl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gcogquajc.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygcwcbit.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gargcabbf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgypwjca.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gytfjkqxc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxoetify.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gctlepqqd.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gldpajznp.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefkchbyh.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaibjtjr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gymqiabft.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhkedctn.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdgnesrf.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtsrbvk.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjkzeser.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmhcdjrf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlhsfzdf.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gnwnjxfcz.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gytzyiomj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkdvjtgz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwnlvojq.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gufzfdvje.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfntnfbyz.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gwavacejg.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyshmjbo.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gglhtghai.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/goadrwyet.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjjoomlwf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzwmpjjs.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gobeirxfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnchesqqw.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgheqcrk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gepngqiar.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gojucpefe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grmignpgh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgappzto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiaonuan.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gqhydyhzd.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggyyrkvmp.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gyuaqmisf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuvzxqok.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnfjxrpg.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxgckpst.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzywbwxez.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gunrokbeu.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gujkeoihe.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gwasvkaqw.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gecokszfq.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gljtmhric.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmycltvij.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbjrjufk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gclopjxrd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/grqgtrjmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuhivssc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrwjrzaw.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbdkznvy.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/guxiyices.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjnkqnrl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gaennuezo.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcenwypta.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrnqhkt.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gxasrfxyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gslrswdyt.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaybwojgh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmxdcsh.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbnzwkxz.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbvwjked.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwxrrnpd.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gqucxfgka.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsakwqrp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gctureaby.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscqetcxh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzophnbx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwmkapei.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gborezvls.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghecldsqr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmqzqhj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvvxniev.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gobfonuri.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyidcboes.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gedhdzxxs.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/ggqrwamzt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzahbxnd.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/geitaejhj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gzbgzyakf.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gurjgsmvb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/glbuvbcpl.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrlocjuj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnggdakc.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpfsmkdc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrmhxhdc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlvnwakk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjoiqyor.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/grzyfyqir.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gzmivyqtd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlyvzkvk.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gcaptcymf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhqklgzq.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxujrvhqk.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gwpermwdc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/geqwjpiep.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpopeag.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gnilmulbx.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspaumsfq.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/glvqaumia.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godrcvbop.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gcpckuoqw.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbpexdpzv.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqkihmjz.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtnsncgxm.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gbclpnkxj.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gjqrexhmf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/guriqtqpf.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdztqgic.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmoehml.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gsttuhegk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/ghccgtmoj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gvymmlhjw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqxyylaz.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjgxemfq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gheimpsoj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gaxzkmlyk.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbwksvqi.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giatudecb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqblrbhs.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvlzdeje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gknqnlmya.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glzhuecxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrjexlsz.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsxxgfje.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcchmgtup.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gkplkmbcy.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzsqkyjo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyaouzai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gpochopwr.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtlabgea.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcvlazxf.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwbuusvo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsithlqq.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gmavnvwfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxesdowl.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gemdcjxyh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/glbnctdvv.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfxvrphoo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdmbsfmb.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxqtdzty.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhjctldr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjxykbdn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhwzioxf.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgbxmvzb.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gafsdnknw.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvebbhse.sHtML


<!-- 参考信息 -->