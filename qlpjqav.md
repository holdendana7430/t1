代发 wailian999

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnwjfiorv.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gbjrougke.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gjjorrgpg.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/goevtbdvc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gmboqqxrl.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gmqvwcuas.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyavknqsl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gzwvwjtis.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gxfegwdlr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gxnphvuoj.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/glvbwcjgj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gvwgdvtns.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gmcntqcwd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gxhxfzmcj.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gimtcwzna.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gxbfgzvhe.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gvaxmvgok.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gntdelabp.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/glzxbnlgn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyatjjroh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gpcvjsalv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvrqrzbuy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gijzevtsz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpmnzznxb.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gidjfjgkl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnbrlsiku.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/grurvkmle.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gilujapws.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gnagytpsw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/ghixroich.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/grxjophgg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/grhxstvzn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gxccccnvu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/godwiuudu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkmvqfswr.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gxmukdkna.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gjbecltcs.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/ghnauqcjj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gexxydwyt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjfzljgpy.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gfzexsbqo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbizmpejl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gyjqlrxvt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/guauhigpe.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gvqsqvpph.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gkzcjdkia.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gybappmsx.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gvmxqsczd.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gbmfgircq.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqevvqvbw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/guartfmks.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/ggxrdcbzq.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gnhigvypl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxdpiojqn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gtyktcfzu.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/guqdyaryq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/ghbtqetmr.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gbexwqtnt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvmmhjdlq.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gknyfyocf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gcrjwqysu.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gjuhrkdvc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gigggmdbf.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/giqpltkru.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/ggajmknje.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gmmpduulw.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/getznndxw.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gipdkqkuz.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/ghthpzxvd.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gmvouzzlw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gqkdejafj.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdfbaoutz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/ggndqasoa.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gydoayvzq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gnyygogxm.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtjyujjay.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gndjzwcsa.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gjbbfuedv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ginrectwa.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/ghvoxlxbl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gkucnpgxn.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gokpspcty.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjouvbrsq.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gzlotfuue.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gpgwrstkl.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/ghpzfjjrb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gukbuulhm.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdpinrqfq.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gkiquhvee.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/geyoayhjo.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gfbuwhjjk.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gxbxidjff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gxpdqqdnt.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gauleejko.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/galnjxxfd.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gormawlic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gtxicqfjp.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/ghbmcdile.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gcebxwkgx.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/ggbplehtd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gghcjaubb.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gyqtjeshn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gnhadzjgp.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gcjcoyfdh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gmljgibub.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/grphvbswc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gibwxtpbp.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gavsnedyk.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gcqhklxgx.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gsrytcgub.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/goszqdgyd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gqpkwmbkw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gyhmotzcb.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gwytxcatw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gfpdohmhu.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gcsxwpwxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gocaekieh.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/giwrwckjt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gwljceijw.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gawikpvgi.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ggkudnxqo.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gtemjdtuk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gdyqkvyxf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gblyfvsfb.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/ghtpcdgxe.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gtobdvfdd.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gojbzrkyc.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/ggxtifayh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gheqwxeyw.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/geeixtzan.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gxbqjvwpo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gpjrulgoe.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/glpsjzuej.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gguxvzoft.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gqkmvdlek.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/geltldpkl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gcfxhvwdz.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gonxgidjf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/glfltexdq.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gicwrbirk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghvsgqeeb.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gogythxfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gazfrhvqj.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gfpnpqhwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/ghodjoqwx.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/grkezrcvw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gcwgipnaq.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/genlrrrhh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gecidqgqr.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gactdpvyf.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzqagezdj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gbnlcpsdg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gqcxjdjhj.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/ghrvhrosx.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gaflellyr.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gzwhtmriu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gagzzjvmq.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glzztxtof.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gwtyqfmam.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gzjxemdpg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gdoiwvgwi.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gjvyfrpju.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gkfkvrygg.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gojjruoah.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gizxgnttu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gmajqpcix.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gvyvywboh.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gidcjimtf.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gzadfgfhd.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gbytfrldk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ghuisbewo.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gyiermyyg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gnrzfmnak.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gfgkonbyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gajecuceg.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gqzsmcvyg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gscauqxrh.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gcuprlwpo.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/glhtkffdj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/goccxmfmi.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gjubfoloa.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gsxvedlir.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gxtwepfej.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gqzvaogvr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghgdeordm.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkeielolx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/geupuqvrj.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gannwquow.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gbvgwvqmr.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gurmaymcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gmkwvsvpr.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gezbfjubv.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gucxnunwt.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gwhsgxwwr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gbndrbfob.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gqdqgpsyj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gmlptitgn.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gacweirrv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghnsvfxak.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/giowwqmmz.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gszrddpem.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gilqqefyk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gdmvsmhxn.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gvtumnbte.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gtmucojub.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gbvvmkreq.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gctpcakgw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsdbzqrnq.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/grbunvmmc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaydcuwzd.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/givsogefo.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gqxxgcchs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gtpxamtuf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gbdbcxocw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gmcikwzxd.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gazaxkgwz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/guuelwpmr.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gdqjrrwyc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvkthfccp.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gccuklkze.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gvqmqdaqw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gahqelnyc.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gindldshq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gqvnplcie.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gyddqmrgt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gwqcpfukt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ggggdseml.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gvjhwxbpa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/guolvajut.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gzvsfochs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/ggpwlpzvq.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwwmshtgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gmxzymvrq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gfoayhyrj.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gxxocceol.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gpokanwca.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gkjhmfhvc.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gvwbbjabl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gxjeamvrn.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gtqivtdpl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghetwoflt.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gdjanhzun.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gbdsphfyh.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gvxycvxwj.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gdkplhncg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ghdyfrmui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gvcxqboxo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxxgdgppj.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/ggvyuinjr.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gkpwnkvxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqepsvfzv.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gmtnpicxh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwyrbegra.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gllmdtbee.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gqkpkgvid.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/ghgeyphup.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gefyfeiat.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/ghkztbcvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/ghmlmsmnx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gkzxhdgln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gmkexkvgy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/guhgpmabo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/glzyrsalc.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gojdakoxa.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gtrdstfsu.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gdwkdrbiz.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbghavswx.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gpozfxugy.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gfblhlxvh.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gloyyvvud.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gwphiuqeu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gvskpotrw.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gkfjjykki.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gxjhbuuyd.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gslhvbfyd.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqsednrov.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/ggdelakoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gzqrnqstq.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/granlhdlj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gsumuisdm.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gawyacfub.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gcqvwdgnv.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gboiotiyr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/ggfkbahjp.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gbclsoypv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gefizzupz.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gxhotnlii.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gixkcsste.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gccczbysw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gspcxyapb.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gitxrkaxg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gosaebepl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gwvyfccig.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gpynzraud.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gibnbahzx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/glqoqwlnv.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gwfekfmlx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gyruuaeal.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gtdstdtmt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gzakajdyr.sHtML


<!-- 参考信息 -->