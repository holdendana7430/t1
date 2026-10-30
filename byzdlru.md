代发 wailian999

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhcxgtvd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjpsyfm.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/glxccmlje.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyaqlljh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyobqpaxj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjxlpzf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/grkhlsuxx.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gizekuhkl.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsyauoep.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoegstgp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gnmrftabr.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhtmqtav.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucylgngp.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/grbfxvoam.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gssmvcchi.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/grjeqksko.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gkpjakpcj.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnvbylgof.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnkdqwxp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvohbjvz.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/giefpmjdf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/ggmmovblj.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gknsunnky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gwbjtowav.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gswydtvtv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gowcbpvfk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwobwtnko.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gfkpymsvk.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdkgnncb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxlkjkxo.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/geewspnvc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmmiffyod.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gerilvabq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhmzfuyy.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwpasebsm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvazliof.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giubtotxe.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glqkaiysj.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxhnuvch.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcyqdsnr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkzuimbk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gmbxwehbp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjjmfdhaj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdigvxam.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gbkxscxmo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/glttslmxd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvyjmhxss.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gfgrgovas.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gggkbidzm.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgxppagw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gelrgzwqo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfdlfakjg.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/godfcsmkl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghruwnykt.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmavyemr.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gpuyosqro.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/ggmxtduou.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gfjblppqe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxppqghwo.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gplxzektm.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/giqsvkkri.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gapgnttck.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gguwztvaf.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gtmvtxrdq.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvzdnstfr.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gyiszkrxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfwkedhn.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvhtvkudh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcagxnzzz.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsngfrjf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvhpriwdb.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gctuwmdeq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorapevbc.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gopiwufsl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdfsbwjw.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gegfntfje.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbobprqr.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsoaimnvq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqcrwkqo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gppsgazwi.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gecmfcpce.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpetucvsk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gynvrjyoz.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlqykbjq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoujyumb.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/ghxzjxzjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmjvbnkm.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfodvyhtt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeatlzjy.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/givcvstyt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqpeidkg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/goixlcjqi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gogknodqe.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/golhqjbza.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glbvyfcta.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwjvntjs.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gphokcfpp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzawbvakn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmzygtgj.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gomgzsyjt.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtmnybkcq.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizygzzj.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsdnahtqv.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcmkvgdo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gddjkdqnw.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkacmlqvp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpdodqjqd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gxyhpzqjg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfxqtojze.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gahwjoaox.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdrcqwed.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gsgnblwrz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gnfgolnfp.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbuziykm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptdwrhjx.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggarijxrm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfftnfryb.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gxlsmvahe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttdijugg.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdilxmalw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhqszmwn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbqumeos.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtewefent.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gebispvog.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhklrqfe.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymdjkkef.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghynxkwqf.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gifvoaseh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/geihpktmb.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gwzbagpma.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/glswmvyfd.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/grduvyczo.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtooylart.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/geordwgia.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjqazzpes.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gnrkndnxn.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gfsnmwshm.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggheqobbg.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdytwjkcp.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbhafdck.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdxyvbbn.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/grfuuoqmu.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjwmeqtsd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmunvagyg.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gcfitqrvo.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxxjqqjtq.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gnmrmhywf.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmrlnkhl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ghzqwfzxk.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gmckqogpk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcfrbbbn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubionpch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpatofbac.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gehsvoqpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghtntigmw.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/goifwpbsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfggvfbxm.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxvzoujw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbcpgbxn.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwkwdwfi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjfvkmmn.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ggcrypwai.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsotqselq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gchortyfl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpxqewjq.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnlgoddhd.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glwtijube.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gmbervdqz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gvxgqjlku.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxugatotb.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmczdepa.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ggnjmqbwz.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gczlyfnpx.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdpbzqidx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gobqfmbek.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gieytnuax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/grdsxruoi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gguvswsme.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/grncdnfro.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqrphxyd.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gewmqkqch.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbdbzemk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/ghearbowh.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkgrnhfzz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gcxjfcwza.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtvkwemi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngypzgin.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gscgpvrky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gmriwggdb.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/ggghobvfs.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/glovaybld.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqeranzb.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grarbfbne.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/guamtaptu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/genhqrgzm.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gicegvvcb.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjstrqga.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopdgzarp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gmkedyvgw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfbkxok.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/glwazhrdu.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gtofftket.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/givadfnql.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnmppgyf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/glooenwoa.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gilwjzxvl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gotrrhfmx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdygqflin.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtabbbtih.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gipyvbwqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdqxrlfa.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjfegczs.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/grbnedgof.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gayvlutlg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwpzfjjcp.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gucowozin.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geyqyaasl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gnrxigkbm.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbyohxd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guoaybyyy.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvselhmk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcvgymbdy.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqygrxbvr.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxcojksv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geurfwrwt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gutqdqdhe.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gdacrpmud.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxgyxjtj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggynkzrjo.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gyqnjqsnl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gzbxhxlbi.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpwicdzii.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmmmnmgs.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/glzonkgkr.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/giyaoyqtp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyekjlbqz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gtxlnnjla.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gyluywwvp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyxpwxgs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpewiekho.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gzidkwpit.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gjbdbmgxy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsvljrkw.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxayemoqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcrdsihv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvazevvtv.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqkwexrl.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzduckrke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfofhgmq.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/glsunwxni.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvivynpw.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyutvtio.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gppjmwybr.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gglycnzfn.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvkdhgzrk.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gsigshlwq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxoyxwgm.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiqorbdw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gzjocsopl.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxhnxzlta.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gfsaozagn.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gckqnyjso.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gijtxrwtq.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gtobmnrrz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmjjvgx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbzmucmq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvultjmjb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphpesjfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gryalktgm.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gadkulerp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddnsepgg.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzujlsgoa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwruprcq.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhxmgpgb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyejsupac.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/glsomxbdi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/grcpvsjms.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gncowafeh.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzuzkxaja.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpoveltj.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvvvjpbe.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpyctrmeb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxstxiqio.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/govxpdjlc.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwmqwvxcf.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtoolcba.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gfmlynvxi.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqttwvsb.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwlpafqt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrljrzsq.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvvqheaku.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/grjjoglrc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdcmruoa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdnirrhz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gudplhzfm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdjayayf.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxyseafu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjrebjliu.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gyziejxvo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkykluji.sHtML


<!-- 参考信息 -->