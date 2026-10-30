代发 wailian999

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnnmeycq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/ggelmlqwu.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojxorkqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/guajotnmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpilkmkzo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gpjmfojsp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuicvlon.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxbscitz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnvuqiue.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaidjsdf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfndmlxxg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhtzloup.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvxezop.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guaywtgpn.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqggehdi.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gjdqpkytj.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/grdngcdug.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gztnvynzz.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gpwmvagrb.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioszrjdx.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvdjzqb.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuhbkmxj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gwuscxptr.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gpjzudrck.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrblfioe.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjetcsyk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gddegyjxy.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvbzcsnx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgncmkff.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwmdzbqaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjzckrddg.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grkqiynjd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfrewtqj.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjcmnxyc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/getosoezb.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqjercjx.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gdpiqoxjp.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gddmxliej.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyaidjrv.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxymljxgi.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gftnchfxf.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjueszwp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqrrhzb.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfxiaodjk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbyqitvat.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbjydkgy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gatitsdyx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcedpubo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmywhdwyt.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvcfhhwwy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grrwtqtmx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfpsbvwt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhpjdibn.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitsefhdc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmnfrxyd.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdbgpwdps.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsosghxwy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbvbjxuy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmnhljvp.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gllktrqwl.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzttuktiz.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvapappbm.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczlxaex.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gacxfdkpb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gaubntrpo.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcndzsavy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpktrdnno.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxxbizwk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggxjambrz.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggwiurese.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/glzshfuav.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/glxjvuqsp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbputixbf.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gjheysvee.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gacupoubc.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfmtomrc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajyxaeqa.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwgllkeh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvjoqtry.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyqsagvc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkpzpbxt.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/geavtczib.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsvwkvoxt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaaypfel.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gcthzsstw.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfigvscu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gamrbuact.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gevvtuhbj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztbywpeb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtmthctpk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gozyrfsub.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqqgessd.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvndzyyut.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/ggxqwzdyw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gpipkcoub.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueazkwgl.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gwtubmwvq.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdonvyzr.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdueoguq.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/goifnvnra.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyfciycu.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuvmvdsn.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqtspdvk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmisfbyqg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemxtqdk.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqmmnawf.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnykavxt.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnfsvltd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gzviouqnh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/ggaofyrmb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gjtjjgkpm.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guqnkclql.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guxagpihu.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gojhreyou.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glgrfettz.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/golzbscvs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gwlujqjoe.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtocdugl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdnckxoq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/guahexsrd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gqxmiezdr.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgypyoaj.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gizyrjyih.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/groigmums.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ghcqphbgn.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gemscclqg.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwwtjzmww.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gckshcyyr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ggheuxjue.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gkechmeed.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/giqzhdsfj.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwbsvply.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gprhnsxqq.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gockiwnct.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/guofvrmsj.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjessbuy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhiqagkk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnejkof.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxrvfhrto.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbesbiblf.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqhoqsui.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/glohbyfll.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/glteybuul.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/glqbkaxzy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gkagiyqnb.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjflleue.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccbhwztd.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmwcfcwqy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gzwrbiobs.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggzotepii.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfwvydbz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvblrloq.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gsdydiyxz.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gefxeskci.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glccfsdwp.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gijscadng.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbkkqifh.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gavpsecwl.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmydjktwk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gktybbmbm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmirlwpnm.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gexxcqnop.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gofvknssl.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqallbqa.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gaqdrlrpx.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudsdbacw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhotgyur.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxnryehy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gsapprivw.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzjqstod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoorbopn.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gmgyuxsea.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gksmebujs.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjhmzyiq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gssckzbdr.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gjctbaauc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glouxkhxp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/grlfwsynb.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwimciia.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwjrqjtg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gafrtowis.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gitsgyyfp.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmyyyfcw.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gbfbafxfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhvekdjq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggrfoazyr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxxwmbij.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gzofvpuvc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gxlczqbvi.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gxfrraojy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/geyjijidz.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grhgjemoz.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwlrsctz.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijbugaoq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjyipgq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhnsdkyu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gksdlgypr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcivyokw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnhoonge.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncfgraxu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gockdmdre.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gkutiooih.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/grrqknyyl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geueljmyi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gbqymouap.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gnteljhlk.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gikkqnexk.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpzrqsgz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtfvvkkik.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gnszsjakd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwxwtpdkf.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gegvylbpp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/geqhibtgs.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gngrnpcby.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gyimssbuy.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gufeyukuu.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gedolcksx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grdczsldc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhjdislx.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghpgigcyz.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gsmotjdbf.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbrrunwj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/govvvpujb.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gibmfuebr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/grsckhqas.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhsbyeif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gspfqlvva.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuhvqiav.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gilsjcnbi.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnjcfjon.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgmmvjvz.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/glbiklyta.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzrpnpam.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzchwtoln.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqidsxbp.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gcwqvmtve.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gficiljqq.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrpegsp.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsovvcmzp.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvawajget.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdmulysy.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gptnggirm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfczfkwq.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/giiguvxxu.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqmrvqjq.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuamcdmr.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxulpxjv.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfbtetodt.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwctfmyxz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdxqhurtq.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gicsagwbq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gevgejzpy.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpcuszjx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwhkyju.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gbaxfdovi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtablzlg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawbqplgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmpbzawb.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvuyuvzi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geauvtxav.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gpcrzrhlv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfmvmypr.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjijclxuu.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfczdhwco.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpqczfux.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gprrbrtqa.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnldevnt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfihnlnx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gffomgypm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gxuafwfle.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyardzvmm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjwmumrbp.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/ganelwazc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfegytsv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvawvpv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmgogef.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaeijyho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwrljxb.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/goivigawr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojdedgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjawaprg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grjylytav.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmmfcjxu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpitxiiy.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gsrgekgeg.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlskzthh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlbwalsr.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gszihqszj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfrmghvo.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwoskzey.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztbsyula.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gcnpweyxu.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhatyscr.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gfktplhbn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrheapaj.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmkcoxwyb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhlbmolq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gduqjzixt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glvyihqml.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/guozqhujs.sHtML


<!-- 参考信息 -->