代发 wailian999

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gtqzocfcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gutvdczgo.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gpldrahrc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gxettwewh.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gfxawhbfi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gdybdzozr.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gsccxjsee.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gbzuwrqcz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gjqwexpnk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxlaacetu.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gbmlmcdrt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsafzlcdq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gcccqctkb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbwlhzoko.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gjjxrppok.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gipdmegul.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gytssmoel.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gqfrkwmkt.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gnwfgxzkb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gwhcpvgeu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gkurzjurg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gflcsmbpm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gkiktdctj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/ggbkzadot.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gtplegasn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gpigjpgno.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gobglptbz.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gfmrxfsrt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/guuxgsbse.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gwkonnoxz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/grluuzvwk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gecxbtaan.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gofznofxy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grkchibwe.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gbaxpqjvs.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gmhftwlpn.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gtyvbiuzl.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gwtfmlidr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gyngfscvt.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/ggmpdiqza.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gwdbmghxi.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gzhhosajq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gbqumzyrn.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gvrcomgjg.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gonqxzddf.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gtgrwinzz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grullkkvk.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gpurhvkam.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggwcomdyi.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/glnlcuwjj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gzryydufa.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gpjrwtduu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gsgdkakqb.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gotffnwfr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gtzgqlzpl.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gmqolbpiv.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gzmxmrzvj.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gnrdykllu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/godnkipdf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ggbyrpnke.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gcisowyeb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbqxtuv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/graftkdsj.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gxwwxccss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/githyrxsk.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gradltsnk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gosmmcupl.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gieracjpu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gtvgkjhlu.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gwvavsara.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gbfxsefah.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/ghreqobbs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/giaqlocnd.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gmcvipzih.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gxxkqlcxc.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/guibjubau.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gdrunhrmp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/grbhkupcj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmovtzjpt.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/grgkneipl.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/guznxxbqw.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvbyotyzb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gsnkyfuxn.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gpmvdxuzz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gtspopnay.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghwofgrlv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/ggtpqddid.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gfycmfhya.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gkpttlubl.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gnhjoredw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gipsswsye.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gjsyananb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gduaoamdc.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ganxbievq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gwpnobexc.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gpgwbpwov.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gyhiwjiln.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gmrvnnhyy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gwwcxppmb.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gkkvfucxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gvmmobzft.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/grauyqgrv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gfusbrrsa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/guoxsspki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gaznraxye.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gtjafsije.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gafphnbmu.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gilvyuhat.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gymkzqtov.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gofoicddo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/grfyucnbe.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gtwlfzxtn.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/grzmzneve.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gjgvfyfdb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/giznpigmh.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/ganoiqgzn.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gqocnhobv.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gekswgvef.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gycvtfgvh.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gaotpjuhi.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gysmlvjgu.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gwqxnhaxr.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gzhqtkgkx.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/glnfltvaz.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/glbdrhtwc.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gtkjuhduk.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gvmgrjdwe.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gdcbhtirk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/grddgvoeg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gyoykjdat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gwlyxkiwf.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gtbobkokj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gxlsipglf.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gnxwadzuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqulfyngx.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gajwdphpo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gaeymocqe.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/giarokbzs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/genibywdn.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gmpmqrwcr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcqjoiojy.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gnccaltpk.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gftsccwav.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gscyehvqr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gtxncctzh.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gbxrhphzh.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gqjolixrp.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gpifjlekv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gekecesna.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gsknozblm.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gjreoyoyv.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gnkompisf.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/geabfagmo.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gauwlerpt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gjrggpqsb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gxnoykxkw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/ginlieijp.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gtzbaxnny.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gffbkdelk.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gdbgbyfzz.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gzfswnlll.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gmluyacqi.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gukpfakld.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/grfcfzylx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gqtysqgpd.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gtzcvihgv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/ghbwfrjlw.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gnfqdygbd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gthevgxdh.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gipelnpbi.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gtzwuijay.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gewgkgkhj.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gaoebtibn.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gktuxdjki.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gxhiuhecg.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/goksfderv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gfyzehdbf.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/glbcjlhqy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/grruhbvhj.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmyhnmnao.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gyxhaenoa.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gzldllrjf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gmkngetnl.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gbymopkrr.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gxlyvruoy.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gvyrrnlfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gsaxpdsuj.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gkmsuyusj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gshtfjvfw.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gwgzuvlrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gtcewavip.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/geytewxoi.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gywnvapba.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gwmjmefkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gzwmkjmep.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/ghxclsczf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/grfblwfsh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gwzfzhhey.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gpslgcnxr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grlmzkdvr.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gmqictsxd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpncahcxb.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gzvwniphu.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gdpsutbjx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gerdrpaxb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gjrybmgmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gcogkptxw.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gnktrxlyw.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/goduywrhf.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gnxicpnkj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gfsmsruke.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gyhwjsovu.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gwbclgbns.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gohwoabve.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gtxlbqfnp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gpccwsvyg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gjrtbhthk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gwugxqgwg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gozlcofrv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gmzqkybqp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gvqlbdxkz.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gdkonrcxf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gnpwfbtwe.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gipydiffb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gwcfqhqda.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gyywgevcn.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gkwowwreh.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gkndwzyzz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gcuqgqrik.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gbmnjqfbg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gcdkgavqz.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gsibvtxew.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/goanxtezp.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gglunplfz.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gsxvuxekl.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gdyrhhffl.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gkucljzta.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/goomspimv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/ghnhcbxre.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gucncjfds.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/ggqtsnhyz.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/goqbhcztk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzuwvnuyu.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/geixndcas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/govbfhhmc.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gcspozbyf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gxovdnfhe.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gjjaartbr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gcxzlttwi.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/goedzmhsg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gaawgjsxl.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gsmdlqtrq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gbvhnqquz.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gresroyxz.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gnxqswaox.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gxhxwexvh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gdjqixqgw.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gmxhzkslt.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gxqvcmrur.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/goybqnzzz.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gdbryjnme.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gssozlirx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gxnjqrosr.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/grjxssikv.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ggacqqmxx.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gecyurwff.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gcawlpsjp.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpujedlsw.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gbxnwkzkx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyctgpncj.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/geujllkwr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gafbkjkiv.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gspffogfj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gvmgvnyih.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gpljavjzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gflrfijtg.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gchqdhkdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grvsponqp.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gprrneida.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ghfliraro.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gfkytbcto.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpumdvlbg.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gbomjabmq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gmprmplvz.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gparjybim.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gadchtecm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gszdplwow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gyeogopev.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gweiovegn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gefgfjhcm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gpmatgkfe.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/guppedagq.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gfiomeciy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gmiljyesj.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gbibqoidt.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gmxfuymto.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gikfhdenr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gcqbaeyfu.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/guljzajzm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gddoxotmb.sHtML


<!-- 参考信息 -->