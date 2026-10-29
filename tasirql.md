代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gvbrndmty.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqhlotunq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbogmmhgi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/getyhkrwd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gutfuoojd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glugkylsz.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gwogryriy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/grvyrdtzz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gmnbcztkw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gukezdokc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ggmwaaysh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gqxomokly.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/guvzsblts.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gcparpzhn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmpquzvez.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gfdnguvsl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gndzbvwib.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gfiuehkga.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gvfysvmyl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtjynaeym.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/grxloivbe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gymaxzpde.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/grcsazovp.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gbheiuquv.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxmemjsdc.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gbvpswdav.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gqptmmlup.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gyjvztfyw.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gwyhgbxwm.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggswnvtzw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gnyosbzdp.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gdbchactj.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gtxlajkhp.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gzpymyysb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gkznfnmcp.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/guahlizfi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gafmvnfqt.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gxsawluug.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gaojhqhai.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gymshghfu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwxmarzyu.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/glaznsjsd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gmuqswmyt.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/geneniklw.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gljpumbag.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqcdrqgif.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbmipkvcg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/glzzbuvsj.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gyxzpcwox.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/goyvkspkj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gzewxncem.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ghrxlyscg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/geoleupry.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gzfhueczs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gagsacoqq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvyitvajs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzzzagycx.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gjkvgauju.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gaubfbqiu.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gwybovvzt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gbuzmubej.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gstwumuwe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gtznttknk.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gszhxclho.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gtgmmtwoe.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gadadhkmh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gtoavdtxy.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gogocavuj.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gupipfnfb.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gjlnufqjm.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gdthgbeen.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gsdfklzdl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/ggzjpuhst.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gwogokqak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gwsbvalsu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gxwxofyqk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/giaypiblx.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gxscgvplw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gpwbfpgfv.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gijwdkqfh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gaqqqboyx.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gfukekedm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gfnbvwbeb.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gbhjomujc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gejcctlhw.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ggoewshcw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gspvvqrxl.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gckjfskes.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gczvneykr.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gwdfodnmn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gkbplviwn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/grxwzjvea.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gbkepipie.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gjqdsrasi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmegjgymh.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gsvmtopfq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/grouzhqrd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gvajscftt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gdbdnzgyz.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gtbrnwvyp.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gguqddmtb.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gevfbwcsw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gloudbrcb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/ggrymcwod.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gybcrlgyy.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gvkbeucfi.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gvkyawopa.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gqphqkyzo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gxblhilgi.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/grerdzqba.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gibcgrmfg.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/grcyhtejz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gvdiyqagb.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/ginbnciqt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtmeqrfpu.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gwdoflhve.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gpgvcmwza.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gsghparmc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gkkqmbhcn.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gnlzeeoha.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gsqoorqlq.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gsasldbks.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/glsjsgwya.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gmpvcmjgt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gzknluryl.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gljxxscaf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnhshcwmc.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/glgiqcdbt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/ggxruynvw.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ggzlsjzlh.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gzpiwhvmy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gmtimwbcr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gfqcdnmze.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gamwbfzyz.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gugrfnbqt.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gveviwous.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gvzrcevws.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/goejsxhrs.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/glluqzgxy.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/glzioxrzf.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/glbycwvbp.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gygqfqocm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gnagjtbnl.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gpmfuphyq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gqhnvdiaf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gfcwjrnsq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gmjvaajqn.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/getyhzniz.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gdbmejhhv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gnuuqnchk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gdtdmvhvh.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/glmnznylj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gxufaceju.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gyzujjiuf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gmkignxzo.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gqsafdewx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gneygfbre.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gzajpgcnv.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gxuxhhqsn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gavfbhhhf.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/geavqlcqe.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gcyvyxccs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gckfgspio.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gmkqyqhug.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/geycsruyb.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gdgjctcfj.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/ghlphyziv.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwrwxaugb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gfnduvzwv.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gcfdimsrd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkrnfvvha.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gfjhjwkxg.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gzmziszdt.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gnvzviwqv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gjjcfnkgm.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/givgfagcp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gyvzccbbc.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gxvllzaef.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/goutykjbd.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gqcmfxauv.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gomnzfbxv.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/guxuialbx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gqecwehym.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gsnpswaux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gftaflina.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gconqpnbr.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gnreooazd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzfvgxbyf.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gezriauoq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gisldswsv.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjbsnmmpy.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gvxpndqsp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gqvoybnaf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/grfhukcgr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gxquzhqta.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gvpiqqjhz.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/ghrnjllva.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gmjtfzpqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gguxdabcs.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gihcwlelt.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gejkalzig.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gabdvldjw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gtrvyrrzd.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gobjszskg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gjfevkfew.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gixtwrmyd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gzpikdeas.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gubgspzwv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gymxcepbs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gyhedpwgp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/grbuijldk.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwjztlexq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gwdbwqwhk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gowxwxyyx.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/giuhnrvdb.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gfhuvhddg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gadcqtbak.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gnewdqgxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gdgaglpbr.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gocicvarc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gqulgrsoo.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/guuizgxnz.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gdtzugxto.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/glojhjmll.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwskata.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gxtbbbwoq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gnktmwdrv.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gbexoywnl.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gbjsbwqwv.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gowdcyyfd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbceemzk.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gciaujynu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkhhosqn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gobfchvzg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/ghozqjiwc.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gejrutwdj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gctolzomg.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gliskwcjq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gnqbraiwv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gfdexwjvj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/glddmpssi.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/giddywtfc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/giwdacewo.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gppbuqzav.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gcidpxcjt.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/goqzsnawf.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/grtivejyp.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gfwsxbggx.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gmfnricoa.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gktaiusmm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gxdweqdqg.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gwhoexmer.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfkictk.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gxvkawqyf.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/ghljhutih.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvsdoaddk.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/geujxogbd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gvldpazak.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/ggumdevvg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gjmvylplb.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gpdylwotd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gahqnjlav.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/grrxpkcpz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gytwutuxj.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gobcpdjoe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gwqotnlzb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/grptcvduw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqoaeisme.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gutzyckgu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ghwtkzeqi.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gabnkulro.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gccsqldsi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gexxotsbk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gszzeuavx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gacltqpql.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gcuekibpa.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gdxjsxril.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gvlxgfvih.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gjqdfalmi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gyewdwvzb.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gupxdfwmo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gqpmomymw.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gyginitbm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gklzetdvv.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gktisbgve.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gvtaonngz.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gngmcuzlj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnqodfwwq.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gayeskrlu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gpdytulkj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gkxifjjhy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/guailfhft.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/ggvpqzqwi.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gamxupfpi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gjcftpdhm.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/guspijejt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsdmagzmd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gqvidkitc.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/ggqkpxtzd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gfbdoqepe.sHtML


<!-- 参考信息 -->