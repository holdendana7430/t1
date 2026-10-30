代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpuffsqr.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/genaxbpvx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjqkcnla.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/ghyehoavg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubmywjzg.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsijlkj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gxstynvzo.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcpaedqn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gqmubqoqc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsxgdqha.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gktlgylvp.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpuuvtoq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkypdwtpk.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxxrrtqkl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzuedalsf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfvilhpy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrwzezhk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gqgpuburi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gdjtwdivd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqxehkrz.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpnjctfb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxfpjowg.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaltmpcf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjoghbat.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzddbgzwr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gphcdaucv.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/glbeqwlvs.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnotslmf.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gpxioabsd.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpmsnsft.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifzgtlyh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfutxflsh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gqanksgem.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyccqlue.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gakketero.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtbivzehc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvogxwkxb.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/ginukpphw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiirwgmx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtdvdhkx.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gddavdulu.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gwuwqepel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/ggnnwpbis.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsikjnjey.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmpdwjpv.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/ghagyctfz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gijxymmqj.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsmqwulx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbzoepwi.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnchefazh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnmrdhmyk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/guylqgxqf.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gtigdygqc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmttennz.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gofupgkgr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhiudnjk.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gdndzrbpy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gfewmchkn.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjnennc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxnhypsd.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzafptky.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhwbixka.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzouprezv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/girchhblp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/geemadohn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glaidgras.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqahbwgqv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggtntmgre.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/griunnack.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggaalhwzs.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/glzmzqgyu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcxfqxjp.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gitkwpotv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gkldyakjp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gazspngvy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwnmeyn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gezdbfylk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwatldmpo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaqyoqkf.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgnwqxak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gybosukbc.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gdhsdjcme.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbqupzjm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gndljppbt.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtypzhsak.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gepksxrbx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjxloyez.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlzpdfbc.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnylhzqn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytxfubgw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzyidvwp.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpjbxrdu.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/grnegqfht.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkhlblgz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtszmprk.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjgjbjgr.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gduzfcbae.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/geieybliq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjepwhp.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylsqfzev.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glgydrjwc.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/guqkyusce.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpmesiih.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwmlbpbe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnapaluob.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghrncdzct.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxelxkzy.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgxrwdrz.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gqkbtysoc.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/geouryxda.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/geyzbyurw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gixmbcsvr.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueliqgca.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggioknguv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzucfgwze.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggphawqdg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwkmjffx.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gbzopxdhs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gagmgbcqo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsosyopr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbdocaxd.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/grktpdjqo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gowsaylur.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgxbiunm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzhjzmfo.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gyvwmogxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqpknbv.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsytgbqe.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxtrinoz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaznckpcb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwhlahcvc.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glpqtybno.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwrzwbwc.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gatgiizpj.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpocprkuy.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwfheekh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzuxfyxn.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmynwfzu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/grwgnpvmk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gompbcyus.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ganhaizus.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gesqwcrqz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjydajoeu.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgifasjt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqbqbrvb.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkbxobfi.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gerqgwwxk.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhsifeac.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glhmseygf.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ggibwblad.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gochcsskr.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giaabxgyq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfigcdvxo.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzgswodh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxamrtvzt.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gptnvscce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gobtdwjzx.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gkpbnpcmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiqrhlti.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gztdmbscz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/grexvnqci.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gybfyhioe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaroshqc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsholrkj.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwcapxj.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegruoogt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gertkzzod.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gylpiespx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gflpbpcwe.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqsiwffxk.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghupbwlqt.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpauiyod.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grxvdaces.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssclxvww.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goagefjcb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glopuzqvc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvyvbaqo.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmleoeren.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gfxixgfhi.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqekkpml.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfyhahkx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gnwociyul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvhhcryc.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtvnpxvil.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsyjjbwy.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gialtcgsb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gllbxbyfn.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgojsrba.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/grgcuoxbj.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwleafctv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpncjejgq.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/grnkcqfjs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqqzdrnr.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekygaxiy.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gegzygnet.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqaieag.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gqxrfzpmn.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/goigihjau.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvldayua.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdxihzfy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gaojvizvs.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glluoakhy.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkepuwdy.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gluijniqw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gzebeixhk.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfrryqua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gqfcnsyzl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakmbczct.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grxvrhnuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsggrqak.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/geaawrxzj.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhiyxtd.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxbvnhfz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgrapato.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gysdoculx.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gmgcbbnrw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/giyfngguh.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gfsukigll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gmavjjqru.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvemphtj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gxagyeuql.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjwjfpgje.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gsydkzovc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqjlfjox.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscilyqwa.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwolrgzpt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gukaskprg.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gkuesalwf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gghskcyhd.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdqvovoi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnoecfre.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gywnhnlee.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvzyximl.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gzoheulbc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gpcyknieq.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gccicytls.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhiauswr.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gxehgmtip.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgipuept.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gihvqdtmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnitqxulh.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnleuxybd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvqrrcnp.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqmirqvx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfmsecxk.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgorkxip.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwkhpgwu.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gfctiqgjg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/geleyvgfz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnbunfcp.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gshspxrve.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glfvglvhj.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggeuwoxrr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghoqlbydx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuwvsrgp.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzksfxdl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaewbprkj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/glnrupmjy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gqufglryb.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gazpeoqdz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gocvtlufx.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gablwsmsh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoafaxvx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwwvyagn.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrsfstam.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gubojpegj.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gkmldnlgz.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnfgmxeyn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gmvhohnrb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjnjqntc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkrbahqc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlbpxahp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhunpykk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gderngdvh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grldbbjdv.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzhlthvxa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgywydbk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayvdheyp.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gctpqzdkf.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrlxsfcn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjoqbcul.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gruxjtenu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gokroasjy.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gogtrjdfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gchwiwlek.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmertlrnb.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmxvapya.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbwynbgq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefrzlbdj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gypjwousr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gihykqvjd.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjajxpnj.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtosnmha.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzehsjrup.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiopyhby.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gzgjhqvia.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/grembdtyl.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gaodsnecg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggutrbugp.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/grwrxtols.sHtML


<!-- 参考信息 -->