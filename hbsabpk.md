代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrvnjdmd.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gipbblgrf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhdwpvbu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gnwjnrsql.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/groaycvxb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqeltjox.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzwabtbe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gachettzc.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gixcorukq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyyiuahs.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gpfnhxhex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaqqyzfa.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gabsqinhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjzdqyie.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlzpgyd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grmhwgqgb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdoensvab.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxmrsiir.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggimjvwjg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggadtemcn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaxopbca.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdjowmkz.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/ghvsgdmrm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqrbnkde.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gycxfviwi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gbvcbndmo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkboonued.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/ghldupxtp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gbqnmeqvs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmnbcqn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghcstcgdg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhpxfrr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gmbskasyp.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gtnjjeyoy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/girucwkce.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtytglaaz.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwnnkpby.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gujrkmawl.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gxslsaapb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsookjws.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gaczmvgmj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/glisgtchg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpjpvnkj.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyydxpgi.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyletfiq.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvpnwvyn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrzhfony.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkjeleth.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqfyobli.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ggqsaswwn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnllffxgk.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhyrrgxu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnxbscvz.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfcmljsx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdmwwhlx.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gulqafopr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaaqbgoa.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gyookakxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyhbhpwp.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gbqygupgl.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncqerhct.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbunddmhw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjprutywe.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/goowemszo.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/grvgplatc.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqoxbyadg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwlpzghze.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpsodspkv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhormiol.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpbtkovk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghxuadbgg.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjhszvmvl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqyryjdsg.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdagrbko.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiqhkydz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghadkczga.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaofskcql.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gostbserb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcakzhncu.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gprfyhchz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/goktuiuse.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtjlyrap.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbpnvmvhx.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdesvrlya.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gukkbhqym.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/giozdppfr.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzhasxijl.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwukotac.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkammkjfi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwburcz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggkpzsrrx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gbdfkehfa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqitgmxzt.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrgwlqbi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/givpjcruk.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipnehbu.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsnzrtmq.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gmtroatch.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbdkmtgu.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagdcyqvo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcxgscxts.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstgpgxkr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ghclczpjw.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbbliknu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdaawwv.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/guefvffns.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnvykorbp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gammnuzrn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gwrpmknak.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gudiigtmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzddyvvzn.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/ggoivutah.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gyobvvrft.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/geirjxoku.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gebdujzjn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgvkxpqe.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/guragqwon.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjhoijpe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjcmqwpdj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfocwzztf.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gstqmzlpa.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/guespgybb.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grbucfvhw.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gudbzqtab.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpzffajm.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwjimnog.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwkgikfn.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfleguuat.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ggwbevios.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbwqlzsb.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/galbhijgu.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaassiezs.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuxyssvc.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gzmgqgrca.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyydtgfdv.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtasmyfvh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geuwbdhwi.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsnaoqpj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gidypmuyh.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaueudcz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ghetjxdqa.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gldstftqo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqvtrvsg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godtliygy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerrqdvcw.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyklatofk.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/goshbtemq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/grmwxhjex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfivbqqrm.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdynfsvam.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnndmexno.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyyudlcd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ggrujtmwl.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvksudp.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gwibapsth.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqquniig.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhffords.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkodlozi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcmqvfe.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gqtumukrd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbjwwjqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goeynwydd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/guxpfzzgc.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gkzvxwppc.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfqniogu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqnltgmk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzjugezm.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/grfkgmhfk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gyvoodwec.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gbytynwpj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxevrsjtf.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gitufqazr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtexouxq.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gbtgjtjab.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gfybwximz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gnmllznsa.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gxywwzyux.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gybnlznrk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkxhtwpye.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhhrczn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviqrcosi.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gqtrnsypq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfhvzeb.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gcoiifgfk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/grrhayrhe.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gjctgjzdg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjoubxdvd.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gellpgyyj.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxvqhqpj.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhmsfhs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkxmzscj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykfgozug.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghorjvzya.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giqoqiqft.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gojspopej.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gexvipaxk.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gnfzngidx.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/ghijwaamw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjvuedzeq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvkrhkwx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfdtmeawy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghqcmuwse.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyfnmlzk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdqmzmfgl.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/guebhsvrj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxpbcgto.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuxvokxr.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsksxfko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsomziif.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjgspxjp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/giffeqjwv.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfhurezrt.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmqqjgjd.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegaaemyq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gislmjvuu.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfhekeor.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzacplffi.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjdbimrj.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwjgpzoe.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/guppgfgae.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gxevazdff.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqqopgma.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwtgywjn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guapxvxho.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gtypwsbbf.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gupnzumhs.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/geqmidqjm.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrffzho.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyqqeusc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gojfdahif.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqdzohwf.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxrhyztw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/giirtzube.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnmoafra.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwoydydm.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqjptekq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gwfbvbfuy.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkrnupfz.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghypdeucx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzppruzi.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqaecae.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsufchrhu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwxvhxsv.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlfysxbn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkfjxruh.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/guvsocwii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyembhgt.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvnwhips.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdchhyeas.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpegbvgi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqewoexo.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/geffdyald.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjajhyxa.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/guecxqyhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gihnrzqfg.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/guvfrbfss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gfsngsfbo.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbpxjgeb.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcevkteap.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxpkmujg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkaqvloof.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gyirksczy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqzfmrdj.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjjyxpbuc.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpjpnlun.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpftcmabc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhemknrr.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gixgftrep.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/galuqhwrg.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtcyeunit.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/ganmfzsju.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqftkinj.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gelwetlra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghqpldkpl.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqgzqsoz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsljetdxs.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gruoapktc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkdkjmjp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gnzowkdyi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwgzqsa.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/grnrbupmi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqnaofjs.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnisnibyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcoecnsy.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gokkolrrz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ggmznghun.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gnpzyhvjx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczoxdxax.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gpdzmfbnp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/glpdywpfy.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdhofylc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ghzvqvixt.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gipiodmjp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gpxzgmrfe.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefbvaflb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkrrydye.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gzxxlnorl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgnniuqa.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/guudufqen.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gejbdbubt.sHtML


<!-- 参考信息 -->