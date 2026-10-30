代发 wailian999

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gncbnxkoh.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/getuzyytw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gwijzzfuj.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gegijxamz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpcwwhhz.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gqevtwklu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gspnqwyoy.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtpzikxhv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuuchfgk.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlnaektz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsnphfchj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gndtltjwo.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gzsghtlcy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbgifvgz.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gimspjxmu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gennhqapk.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gjygeioeo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gsutywxei.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/goueqghdc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gerutwogw.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpooufjh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxsiyble.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhniyaau.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhoueewl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gptxxhijx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbleknrb.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxzwpactv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grialjmuk.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbwpbxnd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaofedla.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gtwexuccp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjqnmyak.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gpdsljgkn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/grajicaps.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlkwspqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfmnufn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/grnypbsqd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyswdtlh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gelfsftqy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/grsuuwipd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoqboczb.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gmarpeixc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyylmrcwf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsamnfpwe.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gkykmtyfo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszocyhqt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gepfisdfr.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gbexvehty.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdztqlrq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpluvabhf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gadzgdgjx.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giallqnhs.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabkaudbm.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtlzrufi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyydnsmzq.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzeysojf.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqvwwoyu.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/goxlbyjfr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzosggsht.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/grslgbcuz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntsxbtlu.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrbbwcqq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gyalrzgsu.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyxhxishz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gzarlkvrz.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/givbuvmrs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gancclmmc.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gpofwaijp.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/ganofmmiq.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxtslvghh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcatixnli.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gdocdighy.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gpzcetseb.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/getuyocri.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqpzyfmty.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpelloiw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfwacjhqm.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrdtkwd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gruzjneme.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcamgysb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaebcdnay.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyobzdphx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmkwjqh.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqffmvjn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gseytumun.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gjzjudiht.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyyudqtx.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghyfzwyub.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gppplvqst.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlbftcz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohzzfyug.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grbzklmcy.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgwgnbps.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/grmqtezsu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujljakpu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnrjazakk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gehxixadv.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkytwqav.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbkxhopn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzgrjyib.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gronhultq.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyblishen.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwfzmyjj.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgtypbyz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gusmsejcx.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gqbnykxmg.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmfhexrp.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyquhhpc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgkowjec.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gvwvltfyv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfacxbfef.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaujnnnie.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbbpdnld.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtupgczv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gofwvijwt.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gafurtyqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpvgqezt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqunfqf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhgmqyhq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gdndflgfn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/geypcqefr.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfilmonzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnqbzjnn.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnkctcqah.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdcnfdqt.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxrzfnca.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgqotcbe.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvkygmas.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqfipdup.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/guwujarok.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gokzzejng.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggdjjcmxf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliqhsmqa.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyptejws.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvravfdgr.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqiicipqr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/girctwluy.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwraohvc.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbfpgexp.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gctfqdzae.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gryorbwjj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giixxzsyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnklktuez.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grkmlbtue.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtrmhrlmk.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvxqwvnh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemdblmy.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gywywcplw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gbcxawant.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gdmfcvsjr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxectvtmo.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gqjuoygqt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrykkgjq.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/guksocjpj.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwsoswso.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmlxnzwd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeavqooy.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkunfafsa.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydmlrsoc.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gbbdddxnx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzezjfhj.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjmmfqua.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdgytmnf.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsdyrmgz.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/girvskrqu.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gasqiydse.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gftygmvnp.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnevghij.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxrdvxbyl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomnbqzrt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/glnrwbjwu.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkpakbxf.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirnapub.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gftfgelkl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhmtlyhl.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywdkmvje.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gyjbpmolb.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdyhuewpa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxmrfyzl.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gzwwywqux.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzceontpv.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gpfdgisdu.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjydzrtof.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzdiznpi.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/grvilkzxg.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwbldvuj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyftlgyh.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gjzfgvpez.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gismapgrd.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnbmcmza.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gmuzmsivw.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/giffnzpud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gfielkbdd.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gbobrqcts.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuyplbtq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcanjpnys.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqnpqyi.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlkucezc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzgvvxslh.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtinmya.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnaxyknq.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gljdefqky.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gayxwhrsm.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/giuzgeqvg.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqvzmzxt.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxowghby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxlqpfjr.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gzxgpvojm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gldidddwa.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkyobbca.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gctatupcl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gohxcmtlg.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbvpaxpm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guzffahsv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzdvpkek.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgwqmjyu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpazgvxca.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxouefwox.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmyhajow.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gafgymuxq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcocemoy.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gsljxmipk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gqkmsbscl.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ggqsqfpjg.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsusonkts.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqyganbm.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gifpqayoa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtzmmmfx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gdwwhnxzr.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gpcnpzeeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gvumweeyp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvmggqle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/grthafcts.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuwrqnyt.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/glhwdvzut.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkyhayuw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gzssdmlig.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdoprmhw.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgjhqdlc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtgfhtifc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzshbqty.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gymdeblot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzyrddic.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/geduqowne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/grvbpgblm.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/godcmiptx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuyyvaaj.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gygxtchfs.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdqxobuv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmlrgufz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsqhwuvn.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggpmnmtmz.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqkiahrz.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gofxwdfhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnxtgcnm.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/goxjbdbwb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfjwwwym.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gtbewrncb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxntekkz.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/geviasyea.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/getiotsfo.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gxbzdnmwp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixpmbls.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/garrrauki.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gggbayzxt.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqmpzrugn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grttdywsy.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjcoxsnn.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxicpucix.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gemztyqqj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntpcfwhx.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxgypomd.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkunifkg.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkinmwzk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfdcihxh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdzfbqkc.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gipvdgoqa.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gjyhfrxre.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlacpuq.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grsqqiaad.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/grflcbllu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gefceadxa.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofmdvwfq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/genvzyxxt.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgrvpzb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdcyomgj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjrjoefl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gshpushnh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/grrqsxoqi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghvkcfyge.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gobuojmxt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/govmdxpbo.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ghohsntdu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfbckylv.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeubonep.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/guftpeqsy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimvholpu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfzsohbm.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gagsahvzy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrsyznoa.sHtML


<!-- 参考信息 -->