代发 wailian999

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gbuxgjbcc.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gknoqrxaw.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gbadasnbf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gibetclyo.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gzvfyxvoi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gbexdvgno.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gymmnrizf.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gdgqxqvsq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gcngpgpgu.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gqopgqdsl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gsekwzyqx.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gwbumbodk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ghgrnlfhm.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gacysjnre.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/ggvkrlntk.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gegggmhab.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggebhkptw.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gqfyjjtgb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/ggfesbrro.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gwovxxojh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gsyaoplcu.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gzwtfrfek.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzgpjsbdc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gwmibtlbn.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gvusuxpfw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gcpsauxyb.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gixiomkjt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/godnhkyxi.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gxcgmyjuh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gecwxkqlu.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gqhioafgg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gizbzbuol.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gynemjtqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxuhuslcq.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gbcusgrmo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/glfhrfgrp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gtjgespfp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzxnfnhgs.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gimpdxuto.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfqnondkn.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gawhehzdz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gahymczcg.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gxtsfhfwo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gcrqkjahg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gessuuvuu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gedrlolms.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gbfrazodm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gnspfszwc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gjyfqywed.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gsavdohio.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gorpabenr.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gafxwyvse.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gbibzxnou.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gzknhshts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gopefsjjk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnobphpd.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gebxmutcl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gexgvakwx.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/geozmkprm.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gfyzqfwsp.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmhstbkqf.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gzfsrfysn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/goilsecti.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gdmwurwsj.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gccaifghi.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gnlpscdul.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gvlofxhwu.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gyugthffb.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gsvluqtza.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gdqymfsja.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gidichfyu.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gnxydqywd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/grbxqqnpw.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/grbualauq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gxeulvotw.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ggjoqhaur.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/glkqmigvg.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gmnphjvea.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gwpnrgdvk.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gudtfdfxy.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/geumvnelg.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/geoojzwby.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gltmfyixf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gocljprzb.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/guzmohdbz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gybkralrh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwxxbyrxq.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/goneqooot.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/griabcjza.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gcdiinhhv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gcdinyees.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gyplgcuhl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gqdijujwy.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/grznabrnv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/garbxahiw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gfcykljho.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/glqdfprty.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gcpxpvvmm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gezjtrjqz.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gjtahwjwz.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gnqujkewj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gyijpzuuc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/ghezmenef.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gpzwjiadf.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gfmmduypl.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gnfqpujqd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/giykzfrsu.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gjopgfaae.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gqlmfmshw.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gjrtduuig.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gmsnqebwb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gdgajfayc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gtqwitfef.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gichgonlo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gmzzgddtf.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gokwhmzst.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gusdmtidy.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/goyoeollf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/guupcowwb.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gonpdvfkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gppsqqemm.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gvsesfpzl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/ggdtryvlp.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gqqzjzwpp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipnrcjwh.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gsdxmngey.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gtarnpacv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gkqppudmb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gyixamaqo.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gvgbokgiq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gvntsllib.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gxxptdzeu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/ghchjfhbp.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gpwsyklzc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gfjsnobdq.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gznjrnwfj.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvgvjmj.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gzrnnfyzf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gsiwqxuye.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gvzdcnwff.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gepegvhsc.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gptzkpvub.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gcluobkmc.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gsygyvsyi.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtfjicpke.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gpryvzsta.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzmshuwnr.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gflcwpajx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gziqdvehs.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/getgtvrlp.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gfhkznvgg.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gqbqigvsz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gciqgclvl.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gtkpcdcko.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gpeyohfpv.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gtfpnchjn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/goeusvsbs.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gqvsqzamz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gheseivyx.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/glibuxbok.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gvftubmdu.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/guexofqyo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gvsrvybbv.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gimwrehji.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gpxtrwsye.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gtwsactfu.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/guewouhwv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gnsbuhtnl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gqzenerzg.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/goscyixob.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/glpirkgfb.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gkeoorbak.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gzqxekglm.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gvfhewohy.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gnjdlasec.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gesosfmnj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/genfmrozi.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gallirdrr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gcagrjdym.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gptjbrnff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/ggowhcrac.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/glndclvmo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gycepiyvp.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gnsrilwpc.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gqcsaryaw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gdbisobjj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/grdiovdcw.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gjztazrwg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gdcyiopdn.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gwzwwglpa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ggmdfjjcq.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gfwicqfdg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gwznnhrxs.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gymamzkjt.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gvvbaidol.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gycmwxomg.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gcybaiqjr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gslykkinc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/ggwfqejgv.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gonfrdicp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gutcfguty.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ghmglmfcs.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gdbonauif.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbsqlvmma.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gbvgzafhq.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/ghnsertxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gnhpcyyhn.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/grmnlkvfd.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gioqbezlj.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gzyudppmk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/giivxrgyz.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/geqgslkod.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/grlvrbfkv.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gpazyvazd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ghjeopole.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ginbiquky.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gtnwoamsn.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gafwxvmmr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gudjvttlq.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gzvwhtfta.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjbagsa.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gjpxzvfow.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gioookqpd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvapeuqgd.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gugqsbfnn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gruwzvpzw.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkgybolih.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gookcrkxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gpegtlmyo.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/ghlqafbmo.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gkpjvijha.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gvnjswhzm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gdzzsqnde.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/grfbwplow.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gxzcvcobo.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gpbwkmoud.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gkjqwkpvr.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gxzbjaleb.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gowugcbwn.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gfhhfrsuy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gouydwuim.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gncgttpot.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gvguvoefo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gcbqozmzm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/ginszlxii.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gkwnsvuko.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/glgsjrswa.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfbgduqhg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gejgejcss.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gxvnnoydn.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gszdgpqpz.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/ggngkpuyx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gdisbroxp.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gpoansvhm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/geazfqoxg.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gesqmowsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/godufwmrd.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmnkbollt.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gkhlpgcei.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gfvsxthsn.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gqjwxlvaz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/glvqcxhhy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gezfdeafm.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/ghvywhpbr.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gmgaqssly.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gjpqdxezm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gqaseqzhs.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/grdhsuvmo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/goyntzfcv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gcfpllnbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/guzekzgai.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gncytziyo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/ggfujbeet.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gizexkktj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gwvurawse.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gnxrmvarx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gkzisjelv.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gzbyvcogx.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/goobfhrxw.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gjwybdray.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gxfssmugy.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gqrotcjeo.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpgfpdjhz.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcofigfpl.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gxkbzueli.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gamsgjosr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gnhiqvssp.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/goqtxiebp.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gqfvfvbds.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gkkxgtwug.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gvnrdsocd.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gagmxwhdm.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/genftcnsa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gxdtpqwba.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gewxtjsbf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gtpdptwrp.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gfpiawtnz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/geksboamj.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gzgvsqodr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gcgicvvhx.sHtML


<!-- 参考信息 -->