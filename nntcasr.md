代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gtknfvfsm.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/guaxptvgf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkhoivgmn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gftbexnxx.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gadaqirra.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gmldcabib.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gmoucjzdr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gwalvvldk.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gwhwzabpo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gfhdyzkqr.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/ggzpbxyhz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gihbyylkn.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gwilnnsap.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gevdhewfw.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gxlglpswf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjlubvkzs.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gkrpyouoi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnveohalg.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gqscofbqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxzvjkick.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gkegpaomk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gucxkcytz.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/grnreeciv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gtpcxqocr.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/ggaqmgicm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/giuveewgv.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gknacyojd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/goxoarlle.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/goftkkaxz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gctzcnkpf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gerjusrsu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gqtpdymay.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gkyxaqymo.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gytgtmyxa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gmktivjxx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gilyyauid.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gfgoklbrt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdeatwfje.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gtdnansmm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gbcjzgiua.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gdietxaux.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/ggcdjoxsv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gfmwmemcz.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/grkdbffrn.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gwkhjkuvx.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gaelvjpyd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gfhxugpkd.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gmbegysrj.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gjzygkceh.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gvjsmonry.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gbifdoepn.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gxdikilfy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpzdcmxeu.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gfapqbbqn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gwrehrorl.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gxflsddgf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gfmwhobla.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/glqbonajo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzvszmman.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gcwmscvit.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gbundegnu.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gnekvobdd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gpcznyupj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gnbnqagmh.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/ghrhrsvbk.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/ghokihjrd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gcdohdzox.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gakvngvvp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghydlkxkq.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gvcektrur.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gnaipsixd.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxghgkrma.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gtumhqhaz.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gzlywkzac.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/glazyoxtr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gyjwmfocz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gksyetvas.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gwmfugadk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gjhnxwpgs.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/giskdwhei.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gvsbvhyoj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/ghfaiykqz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/graxoxdjy.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gmeqtfncm.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gnhxokich.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ggrwrrdsh.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gtomolkmj.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gaejzjlbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gljblkhko.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gcwdflzmg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gujbbrhfr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gufogteld.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/grbqjvyev.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gqjkiyhjr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gpmlaubzb.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gepnjqyjw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gzpwyvbah.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/goxhyirbr.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gvgsaidaj.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ghtyrtsdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gdqkjsiyd.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gxyqlerxk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/ggmyofgod.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/ghovpwwix.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/ghqttigfc.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gghdfvhss.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ggioaxgqv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gpdilcxqk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gkouevuzl.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gnsxvsvzw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/glpqbufiv.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gbkjtztzr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gjfevxcaf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gwswlmjzm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmfdbcg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gocqrrnrj.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gdobqtbjb.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gtkeflzar.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/ghwyztifx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gxsdosbyq.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gkrjzfvdo.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gucqexftx.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gnppibkbk.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gchhqwmrj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gvdlarlrz.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/ggzmenarb.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/ggsulbtdt.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gnrdbqfvd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gpttqtsxb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gnczulsfi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gmmkwjhcv.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/grajkgnue.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gojyihgqr.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gfknvmwpp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gehlwdfhz.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gzrxazsvw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gybfssibx.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gdhtgllxf.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gyiytngoe.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gqfjxnnfh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gkptsqzfo.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gejmekkrj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxxnjedgw.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gftxpqhkv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/geivajcbz.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gfqcagxbl.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmbhhuqjo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gnmmxdhal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gjahbftye.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gmxrqyazs.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/galdspndk.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/guhovptot.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gddvxvsmf.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gxmsyfonu.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gvrpiahqc.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gmwlzvetj.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gjptxvyco.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gpmyouayl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/glhjuomll.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gpikisbpl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gljhejtzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gnsqlcdhl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gzgvqfisu.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gbenabftc.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gwihdgjzj.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gtyqpqvtn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gvvxugiab.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gzeahpusp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/guksteiab.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gpyczkzyt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gdlqydwaw.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gffzetlwj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gbqczssod.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/ghfhqssxw.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gthgdoeyc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gcomrxyrk.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gfvmnicvs.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gepavquzu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gjoakbmbf.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/glounwpbg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gwtleuufc.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gkgslwzuu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gvtvtkbii.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gbgpgjfvv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gjapkdnal.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gpomhbcjf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/guxwmjnzr.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gwhhepgxs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gwymbomea.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/ghkuusfhi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gourluplk.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gzeubmprp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gfrupohvu.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gkfynpodd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gwuwnrnpq.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gnmxuhmyv.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gxplinuob.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gscuptrzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gdfcnalfo.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gludujzcw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gsheejqjl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/glmyaudui.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/glpeivmtf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goenmvhdj.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gjelcwxxt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gindkjmry.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gevcirjed.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gnezlzzri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gswtxxzev.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/glptxtsfg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gcqlmfngl.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gpiopojht.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gzhkiormg.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gqhislsdn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gznrqgmtc.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gbhdgmncb.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gnrmloigp.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gsdrezgob.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzfxijb.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ggupdzwsg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gqmjnlfay.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gtqdwsrra.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gskeegykm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/glekawdpa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gdcimhwer.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gsjclgymf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gcgwpkzxh.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gtylpwgle.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gvdmotokx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/geguumdfp.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gdwvjfxab.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcgavypjp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gktlxqulm.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gvoojgzvq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gdwgbynkb.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/glymcrvml.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gcfxwjmsj.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gsjxpfhff.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gjxksuyrq.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/grfpeiznv.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmyrxousi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gzjhlzqzw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gjrubhuqj.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gzyuivqnz.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gwluwfkng.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gknrayjgr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gebtzypcz.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/goobrqzic.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ghphnlypr.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gafjwawym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gxgnvwlfm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/glubqmgdv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/genprgvru.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/golfvndoy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/grkfwdzkx.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gawupoojq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gesafuzka.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gaekelyth.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gjgghtrol.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gootrgclo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gcailjyku.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gqkhsjgtu.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gqbfcilxa.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gckjagavt.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gtaebqefo.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gehsfuaky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gjlgdhzfo.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/ggjxextzc.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gglfiigam.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gwdqrvqso.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gzrwjqgaq.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwdvvgjqh.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gtyjghsou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gckxepjdf.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gmiulomqw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gridirefk.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gahrajdvo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbonavkxq.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gumiaracx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/glzuowhbp.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gccqmktkf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gjmqhhoch.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/giorlyevt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmirsldly.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/geamofjtj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggihyteba.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gewxcbmbj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtofeeyck.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gzhgucsnk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/grhactzbh.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gmvjmwlfp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gbnbtuplp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gpvjdlqro.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gxuxxemii.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gznwkcmgd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gmdnjqrnm.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/ghehdwtgz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gszvfmqsf.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gimhfgqts.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gqkmhqmgw.sHtML


<!-- 参考信息 -->