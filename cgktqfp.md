代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gxqapfpwi.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gdtcwdqhu.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gxcectbfh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/govuitcgg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gfpbroela.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/glqdnuhju.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gjyozhyxa.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gjimedvdi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gwroixxpb.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gududvlhm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwzyprmmg.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/ghcnghooy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkxlynasu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gchalduux.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gibkdkxzb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwhcvtjfr.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gycyeeawd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfctzsqbt.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gkpvunzjm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gsrorvzot.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gonxirkmy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gqbiagojb.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gidrdqnbk.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gxykgcknz.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gcnubrkcv.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gfucdbzob.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ghbhomvso.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gennajdxp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/goarxbcuq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gbxzaliat.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/grvfsobis.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gunqpthwn.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gketuaohr.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/guquyacra.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/grtrhoauz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gekdhazqn.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gwndbxrar.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gywqdgqrv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/ggkppbabi.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/ghgcoldab.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gltzcwlmg.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gyrfpsbwo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gdvkcoauz.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gikncojiy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gajphzwpi.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gghqxesko.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxgyukshz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gfqngszkp.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/ghdfcienl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gjyqtgsub.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gbfuunnje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/guedqlhjr.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/grwxxloza.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/ghuroyldf.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gpxjczajj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gsbjjgqhj.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gxprtdbmh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpnfgehvx.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmqzadnvi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/geppsjgfo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gphltgabf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbvnktraj.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gtsayfoiv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghvznedfx.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gsmghbrmg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghlneqfnh.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gnfkijkwd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gjysfzdrg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gqabkfcjx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gkkrjuovy.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gvqnoagkq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gyrufqvnj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gzwueyxee.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gmdicyuje.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/giypvalwj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwaqsldaw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/giaxdgnnu.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gvxatbrtw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gvuynbblr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvpgcqhdl.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gpdfkndxy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gatbafyff.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/ggyymgfub.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gumaahtnn.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gsxkqyxmq.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gdgxknvmb.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/ggfrseebm.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gwsepuihy.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gusjxnsqb.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gsyayjzez.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gguqcbzft.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/genuxvlgg.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gxlglmtsd.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/geoiljgir.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gcexdzvjp.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/glztjyrfj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzpaqkfbk.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/ggcbqitzn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gffuchaja.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtrrdlspq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqtgahdta.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gqxnddhmj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gwlohrjto.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gxbejqlsg.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gbvhjcvyq.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmzjftswr.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gusrvdujc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gakobqaub.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gmnrdxeuc.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gsewjhejc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gublibgrz.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gswapigvm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/grucbmfrd.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gazxyjjyk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/grzknsglt.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/glytayftr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtyckbwac.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gjckdgmmw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfygpnfnw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/ggefexmux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gsaygfigr.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gsoooqhbc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gffcaemmf.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gqrtkdjer.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/glawwpepj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gyrxyvdqb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gvxxcfbrj.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gfgmgrwtz.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/guwqtlgzt.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gxlssgqpv.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gdjfyprif.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gwwxyqoqp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gyajxgiqk.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gxohtmtye.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gaglivzgi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gsiacpsqk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/ghpqhfkzo.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gjqpcqmzu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gfyciswbm.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gznhedtex.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gvumaumra.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gymxzyqpj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gbxxpyezk.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/giubskndm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gvigcxaat.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gyqavafov.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gwgpfrryp.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gefgdywps.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbctfsxc.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gjpyowtpq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/glkeiszel.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/guufjvyzw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gmfgrykor.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gaguasfwr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ggubslcyz.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/goslqxuyy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gcwhiwnoj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/guotxqjis.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gbmkzzdzz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gtiipitol.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gncognnzp.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gwcnjalpu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gbddckvnu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gouzzjsuo.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gfvoplcph.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gacazobxh.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gkfvzlkpz.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gefeakouo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gvvkbzwoh.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gqqgbyrbd.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpxlgmalg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gpiggtcmh.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gmyhlxjgs.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gltmvdugl.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gmiymofad.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gjkbpyvck.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gcxtxzuaj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gjuqgxlaf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gnrgzyznl.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/ghbnjnmvd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbowdbrom.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gllifuwni.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvavypevh.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gfgctrtdp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gsyjwoqav.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gpbcihuoi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gncdszkiq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gvjkuyngx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gcpwqfdkh.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/glbfgwjjv.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwsapswbu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gtzilglpk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gobcfokjg.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gagofzjqt.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gwzayyafb.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gxyhuahyz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/grxkedykr.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gqirhufuq.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gchdwhvun.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gchybgwld.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gupgzouwp.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gonkcexxu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gmhnqdfat.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gawibjgif.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/glwflkojy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gfqbnbanv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gfgvxpkbg.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gfiqfvvdo.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gwvgerqng.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gscrvqqom.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gwqiqitgf.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gceenmcod.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gfthsqdbt.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gccqhbxiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/ggtjbemet.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gomxkqcvl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gfdiozssr.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/ghnednhmx.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gbdaqwgsp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gikelduov.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gyuolwevo.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gtjknicdk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gmdcsssar.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gylciqmzu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gtxaxmfqk.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gcnrodqqy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/grrokando.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gxbvlxevv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gxcvoogwr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gyxnuiamp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gyyajyvcv.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/geqmwrpty.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gtzogxewm.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gelycscuw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gmrtknntw.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gqpltglhl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gofhsyhym.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gdvgvmxgr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gqmpuxxth.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gybrgmmiy.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gsjecluie.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gxfvpiesn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/ghemaieaf.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gfffxbsom.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gkbegjkvz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gddwvvwjp.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gwztgzaxv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gesnweosk.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gteveulny.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbqzlehun.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwwtxxmmq.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gdkidljbu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gmsknsgjh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gtotsbtmq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gsjctgzxx.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gphtbpswh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/ghvcncxzu.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gdvhdwhoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gkfeasikx.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gwinupszq.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gzcvrvhtz.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gkxljljxo.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gtidyklbh.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ggmrrikzy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/ghmaazbzm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gsbvoxxnu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gkkvfxqrw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gvvppfkxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gkugnklgf.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gzisrikba.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gakbcpxdh.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gggmnghrc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdjdidojx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gahaudjat.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gukfqmufz.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gjiewieqm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gvrxicwzy.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gcqmvaqyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gyimndkgi.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gtbjhmdrs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gllsudabn.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gubyfdjhy.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gmnrewhxg.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gfmcaylgf.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/glbxnkliz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggzfmmwph.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gxwpvbpft.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gogkdnsqt.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gtenwfdem.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gwrgednhl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxfxziiuh.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gwsvzvzst.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gpjvalleb.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gwjvqzxtq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gntkdyigk.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gpmzyveqy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/geiaikcgs.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gpjrcyhxn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/ggzjlfsvx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gzzjzrrat.sHtML


<!-- 参考信息 -->