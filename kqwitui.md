代发 wailian999

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gqlrdxpja.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/goljdnfpx.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gbcjjmhct.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjqexsmsa.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/ghezrddra.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gztugnhwq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gfxqgfiur.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtiwtnuwr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gisoaokew.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdgdzvxza.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gnrtrxids.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gtgimkbnd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvaodwb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gbgdankio.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gbdohmvks.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gxprfdebx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/grktedors.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/glkrucpfm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghuoyyjsy.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzpklbfqj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gjjndhklp.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gwckpeugb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gdmtquhqr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtzxpnwnq.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gaoithngq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqvbjvcnv.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gqkfadapp.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gbqdonjmb.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gunhtyslh.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gbqyabslt.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gsctuauvm.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gulbhttvb.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gdgfxzwzi.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gpwaiahpy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gzluvatcu.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gnqurvbjp.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/govpebvna.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gsbkoojdv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gtgauqsyp.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gmrkzqjce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gegffzvye.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gzhdiiusd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gabouusgu.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gtdsdcfqw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gbuidfyyk.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gaqwdpxwy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gzqzcesds.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/glnjxyxuc.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gullpjynr.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gppswzyks.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/ggrglnqjh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gctaglzqh.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gvqyrfflk.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gapecuxcr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gqckjwutw.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gtcvfybxx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gimvkhubf.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/glazceyuf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gznrxzqms.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gedntidfg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gljijaryc.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gvooymrfs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/grbutwnst.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gtktvzglx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gdymcmjmf.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gibvfghwb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gnzywazkz.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/goeyloxav.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gqlwllvjy.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gulktnsyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gduwqjmpv.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gkktptwwa.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gslgzqnzx.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/grnrzlmnl.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gikzaooif.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glbdkaxlg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/grjnlkbqm.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gsfdeyeva.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gmjxhviuk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gkjyqsvam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmbktlnhb.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gszsvlptu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/ggffpmhlj.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gmorcshhj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gohpxdfja.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gtgxlfslv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gqhxvzfbu.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbavrzvhz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gaouhvcwg.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gdglwobbs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gstekziuk.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gozvnbvov.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gfrszxdym.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gjbvpalww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/grweesfsh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gkpkmfbim.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gbilemudw.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gyjnjrjed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gsqhrmsow.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gedrykmxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/ghiybsszi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gswwpvvcm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gsoqakdon.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gwutvzunk.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gtonjtvjc.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gfrlfuxhz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gqqczrvgb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gneoddwwf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gumfjcyep.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gjgiqilyw.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gvalgblpn.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gkpdzutob.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/grovopgzd.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/ghqgewgjz.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/genupnevv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcvtanggd.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gghquiify.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/glgpiyzjb.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gxliqlruq.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gpfssdmqa.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/ggtrppxtf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gynkcglnl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gpwtzocuc.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gfrjkzfpw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/goffpvdgs.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gxbgoidfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmbtnzksg.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gdmrsawnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gqfdjcshe.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gtpmastfw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/golxppzxv.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gtpvsotmx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/giwosylny.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/glohjuwto.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnqsiupws.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmyzjxwai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gwghkczdd.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/grzbbdgrj.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/grjhjkuin.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gyoeuulid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/grpwmocll.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gkmdwfnff.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gtikonkmr.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gqovhhebo.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gmzjmlnmt.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gdicgoqpv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gsfcasukl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/giewskgng.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gqvqioneb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gcxeqrwfo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gjblyqflu.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gamfzxkis.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/geypvncot.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gsyyxnttj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gaetqmmkx.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gtcdfzxhw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gludfysdf.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/giqsfwcdb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/grroqzywe.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gpvgaqucq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gvyzkfyqm.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/greljmzmi.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gkonxiadk.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gfuavnhjj.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gleuxsmfj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gofxccuzc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/ghoavgbtx.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gszroajox.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/ghauicepz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/ggrlbhxoq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gblvecnhx.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gesdwxcbt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gnpfonjrm.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gendltsmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gboxubine.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gbhhtfqtj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gyrrfcpda.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/ghhboffms.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gmvthrihz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbjcqcuhm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gluntlubs.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gkbfrnsgq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/guhzvpxca.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gyobtrsmy.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gtmiengsr.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gimgtnpxk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gxpgbnujl.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gwykxbwko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/grnpernud.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gdzbeqyha.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gujijpvuq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkssuikpn.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gjlgeczou.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gunsziepo.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/ggipbxuei.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gadbdpaqj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gaixghdfd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/grtsqaplw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gpidvlqxt.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gwaduterz.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gjcxovpiq.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gajcrloja.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gaekhqijc.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gxcjhcdgh.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/ggiazeqpr.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gbjeibguc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gniukvwot.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gkmoubdpo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gtyhhllfd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gftcprgjv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gmegrzpli.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gszotrezq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gncqwnuku.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gbwzholif.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ggkeqbdpz.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdagyelfc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gaxhooudz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gzihiaees.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glfmszght.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gbiewkrid.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gzipwvquj.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gvfwhnbcq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gvvapooqp.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gyxfrhvff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gnprnyzsp.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/grczyfttc.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/grsnkwfln.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gxqdfxsvy.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/guxfvwdno.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gmieafcxg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gjtstperr.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gprscyqke.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gwucvrwfe.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/ggrwpgkyy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gcfsdjvvm.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gxbvjgnjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/ghzsnbhlr.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/giawoqtzp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gmzrhqoxo.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gayaxefct.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/goyjvuwwq.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gggtlbsim.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gouldipfo.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gntyreifk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/ghkqfscyl.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gyrooutrc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gbiepdaux.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gybbbqsro.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/grmfwgzhs.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/ggoyjhcjf.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/geoikmpwr.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gwhadacgy.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gsvgwobub.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ginsuewba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gbborvkht.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/geoigufgc.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gxviudssc.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gbbrmtddl.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gnjsxwyup.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbovgjdqa.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gbiyadztg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gxwucoamr.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtexacgji.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gusnqyrzi.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gtzkwshhg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gwmdrrrgt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gmtowpeef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gyyllxdby.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gonbfyzaa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gzspvgnxr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gmoxffjgt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gxxvykngj.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/giwuxlxtd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gtzylzjmf.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gttwwhkzo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gpdbhpaqw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/goiwhrbww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gbgwftfrr.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gkfsgkmwi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gbezttcax.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gsxmzirga.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/guycigmmw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/geveovukc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gjxvzgwzi.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/ghtdorqqx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/glnrdqstx.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gdwfxpzxp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gpdsllxdm.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gwumimkss.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gwartoppo.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gyxqgvfqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gsxhdrjls.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gwtoiqgrh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gzfhptcox.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gpckocgap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gwcqbwsmh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/glticozyb.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/goupytfue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gmtrdwpih.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gwgundxfl.sHtML


<!-- 参考信息 -->