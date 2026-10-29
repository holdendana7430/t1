代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gbntnlrce.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gltozxmlr.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkqnfvaod.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwlinapiv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/giecgbkoe.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gaozuqund.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gmqqjxztm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gnomkuugu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gjanjcfzw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/grtfxurxj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/glfcondru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gdrvnkxph.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gvvuharjb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/ggqvkbjbd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/goqemtfmn.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/glocylfil.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gtyooawwo.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gdineeprh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gmjjtwzaw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/globrdbrz.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gyjhnjkca.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcykzyrcv.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gecrmhiae.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gdiyopeam.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/giaeulryq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gfdqgakup.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gibwxorhc.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/giaxiurkv.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/goffyituy.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gccpwjhjx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/groqhelbo.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gtrnvfrvt.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/grgdiditd.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gjvfyaalk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gnpwbkfgy.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gdqleptcf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gepbdalxk.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gormjsqwp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gjrqmhrsy.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/glfbkjghi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gitszvzcx.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gjgnvujoj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ghrvkqnyp.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/ggghdbzhg.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gfjzmtteq.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gjldagrws.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gohzgmksg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gawldeyvr.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gaoofupmu.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/guoqkqodm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gowetgdzm.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gpcjzdykt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gogaklkcm.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gatwflrol.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gcodhhhst.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtivasewi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gmwrmtwyn.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gobbxkzwe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxdnajyfm.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gvknzjcbv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gdahufzst.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gfhmibnrn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gcnkkcdxj.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gvsmuvujb.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/guypaltsp.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gpjyuosqz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gaseuwlny.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/givbsjdjd.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ghusytubf.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gddhscwsq.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/ghglpzugo.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gfcvaylva.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjfrrijrj.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gutjsthle.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gtaxvsbnu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gdkuefqlh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gvnmjqjdz.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/ggpvhkixz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gbkbsqeyc.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gsuidepck.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gsmlemnat.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gxvwpjgan.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gpteiperk.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnruziorv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gbtnohyzv.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gxuzphyuj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gldkoyixz.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/ghlefuais.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/geqqupvis.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/goefbwmzo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ghupoqrky.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gcpxqxpts.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gzbjoosgv.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gldcbqirh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gtaykjlsr.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gncxrczml.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gjwwzvdxu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gauhykgew.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gtvxwcjtc.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gowleogzi.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gnxaajohm.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/grxycekbx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gzwcxjcdm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gczozqyrn.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gtcdxbmza.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gbeftovuh.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gxtwdtokp.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gnoyjfien.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjulerwge.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gbecslkcz.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gfhcmbzaq.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gjtzdepzo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gdfthhrcz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/giccexpgm.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gqdqqvlot.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmwspniur.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gitunnqnf.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gsijunppy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gzivaxlbe.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gemzaawnl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzzenrpsh.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gyeesnxaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/goifkmdqh.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gnlenfefk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/grohfnuge.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gkmcrmrib.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ggfftfbzh.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gcifsqsiu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gbuxvhdgp.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gsuwfdnkl.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gwimkjvzk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/ggesgcptx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gojkqvhzr.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gbfmxeacn.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/ghatqayvb.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gikrbnarl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gdpybkwjd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gvtnnvxpl.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gebxxdzke.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxhugju.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/grbophorm.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gdaygewdp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gouklciop.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ggzhirzqu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/ggzdbzgip.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gmlhygwwt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gxwxanvom.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gpqfeucrg.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ghrtogrrp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/ggowkewdd.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gohfieuqf.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/ghhtkdyug.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/grvcjrqwi.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gkxgqvheo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gvmbzakar.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gtuktxhxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/grgehcjms.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gcfeupbth.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gedelsxtd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gpinvlcgs.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gfzddoeyg.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gpmshntaf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmjaxvzav.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gnoqdiyqr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gfrpugsrw.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/ghouswprn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gdmbfhdvi.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbvqkshnw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gavezpcik.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/giydlrnjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/geymfewoo.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/glagyfvra.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gcuizefkb.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gjduvcvcn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ggesbkhhi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gzlpzfoii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gksqyjlfv.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gpbbzmjkp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvozfulrh.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gxjkzgvhl.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gxqfthyea.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gjrctarha.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gonjipbwj.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gfdfgrjkx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gevrdyqum.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gduzglxbs.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gifzsjull.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/graabqfsv.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gkqplrewb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grhjnxlln.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzhxlunpt.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gbkxthjbd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gjauoxaia.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/giduboazw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gnaueeckb.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gyynwhult.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gyqpxlmit.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gyssgouxk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gcuvuhixx.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gcgjhrscu.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gltgiahtz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gvfdvhdsp.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gubmadrvl.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gfbcbgsde.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gpyciilfo.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gmmdbzfpy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gaurgtkmg.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gkwfyskxe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gywwawsvf.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gamjsuosr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/giaaovncu.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gwldustce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gpeyhunzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gfslrwnlu.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmtauezqt.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ggopjsghl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmnjcnbfi.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gbdocaewl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gzrtpeolb.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gslknkcng.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gtwqlhnqe.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gxwhomfex.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gralcxieb.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gstlrktqv.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gxhiccuth.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gerldahgv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gukclnihm.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/grjlyveiz.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gspcijmnh.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gblhahoqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqhklsbuc.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gfdhgrfnf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/guvnbthlp.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gmszuhqkx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gfkyekmmx.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcnsqgqyg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ghwnfdgeq.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/giaxadlmn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gxpvpiffz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gchzxuqik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gswhvggbk.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gomqitzsc.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gtqeizlxz.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gkuapbrsh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gowqfibbk.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gdzoiksao.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/giqbhpayf.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gkjqmqcfp.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gkcyokgrn.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gqubtutus.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gvtugrmmm.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gyzcaspql.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gvygqekaa.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gkzojztsr.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gtwiwjchk.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/grhiubclw.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gafthtfdk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gajxjqjfd.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gbzvlyrqb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gjfpieoxz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gsivqqkoq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/grdtskext.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gumriefgd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfawwozjk.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gbpeixlzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gpshapotz.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gunqadehp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtpsxvwko.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gbovkirjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gfsbycywc.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gclbuukxi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gzuqhhhaq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gnrldqgbq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/ggyooiugl.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gzxgpfhpi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gbridyong.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gtzhugotm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gnjpsegoc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glfysieru.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gshwaquri.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gtlddxdtz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gbwbdubfo.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gmikxcnzy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gzoctmitd.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/grnybmcbf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/ghvjflayt.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gokpsiaeq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gyvptoesp.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gnrlmoxuh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gtclkcbmx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gmtnypyll.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/geygrtpxr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gktygnybg.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gmlliwwvv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/ggftreufr.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gmsbkuugc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggigasdpi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxyygtfeq.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gzmaavrov.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gibavhogn.sHtML


<!-- 参考信息 -->