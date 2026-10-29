代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gqsdpcnbp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/grqxmokqm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfsvzlccy.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gaflvjclz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gkefvmutf.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gitdlaxgv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gfbwssrjm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gskylzuih.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gezohodtr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbifqfsfu.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gkxdeuigc.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gjebjpnhr.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/guxkdszct.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gaquodgnk.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/ghxbhgiod.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gogenjfuq.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gswphqkga.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gybencear.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gyrkrxipe.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gvyvwvqtc.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gtgosrnyz.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gvfyallmj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gjztltimy.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gehabqdvy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gbmlszbnn.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gdwvdrype.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gddbgzhpw.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gvqshcbuz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/guawrprcl.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gnlpjkwsd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gxvsszyft.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gogswyqte.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gxglnxrle.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/ghxsrzudu.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gjpyqnxgp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gyaxemmyd.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/guqshssbk.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gsyagjevz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gldefjhyg.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/giazymiuw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gneotdaok.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gwvsyrxqh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gbghggyyf.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnmtthzot.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gkmhmhghb.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/grrsqfodd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gkiiscleo.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gxjretcyj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gmxfzrcdl.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gzoiebgyl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gtsmzbyoy.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gkabhrkec.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/grhyqloui.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/groweneud.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/ggditldfp.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdvzzlelr.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/ggexzhorv.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gtgwzbpsi.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gcveqtynw.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiowsgc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gdtxszmgb.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gfboavioe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gxkndywrl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/ggtfhwrqk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gwdfodccc.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gdehctbou.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gcujwkkmq.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gzlcmoiku.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/ghtqxsouz.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gfcgpvecl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gpibyfbno.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/glovbrdvd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gzikqqnew.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gqsyclege.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gpgovrzto.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gtjbvyhus.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gvvkqbrqe.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gijjlhado.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ghuahwkyy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gyqlhczwk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/ggtaqbzhu.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gkdipunvb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gcehbkxrq.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gojeadvfw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gvsynnzfk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gxsiigvcm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/glgylmfro.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvfjvqyko.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gfmkadeps.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gulxzkqmk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gjinkmnsf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gulskltgx.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/giegcxaww.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gxrvmbkca.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gpfkvpsup.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/glytxzxsp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gyzmdsglq.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gdlcaodpq.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gnlxowhhd.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gqyelwuct.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/geaxaqaue.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gpkdcoxsg.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/giikteydy.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gmxppxizm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gdzibeeow.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gjthnrkob.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/grhkwqqtx.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gzpctkbru.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/guyfkyvrg.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gdvpqtgpt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/ggwzaysai.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gqeenidox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/ghigrzncj.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/ggihcnudd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkesxwhbk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gngnzxjdj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gnmkwmljz.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gtuvetdlp.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gdrfqfret.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gpoidqzus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/grzltrtyc.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gmonvmymh.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/geyuhbpzj.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gwylqmebl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/glaetjmsg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gqodhzsji.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/grsyxoxru.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/geutvarsd.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gnnljfvmm.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gldywdzks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gwdvilayt.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gnsmzpkpl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gvlfpcnan.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gloqncyho.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/grageaiqx.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gsscozixi.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grnlvbkkf.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/ggbsepmih.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gajgvfuyt.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gymvrdlin.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gplqlevdv.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/glvbhrpqq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gxlfombez.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gptldnmwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gqcdpepkn.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gweipzfxn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gczorxign.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/ghkzmcuru.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gjmqkhciu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gcrqlodqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/guwzxfeqg.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gyrhiecqo.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gjdfjiyds.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gmviynoxh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gsolupvhz.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gxqeckqhd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gahlatldi.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gbjdktxyp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gntquevky.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gynimhozc.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gnytmpdub.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gtisuqjtc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gybibvtit.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gupvvwpht.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gcyeinnpg.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/ggvelxzxk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gylppvokd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/glimjuwkg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gckkogocq.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gqopuzptn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gfwddmdkb.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gcfnhezlk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gxjkprqnh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gzbmzskwa.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gnvvcnhez.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbmftlvvc.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gtncmdqoi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjrgjbmqs.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqydrjfiq.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gezgguplc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/grgkwlgxf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/givmuzkww.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gpldkkrzb.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gkmznuzih.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gdaicwgam.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gapyeazxq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gzughfqrq.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxkaixmby.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gekhpeauc.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwjnxqaxg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/ggrzfftfc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gduqoivrt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gtvedmbug.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gbwmlzfoc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/ghlsjxnal.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gnssnokso.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gqjobfpbz.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/ggflrzuun.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gudaloskj.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gcwaeccoi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gozudvmao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gqdwodkxp.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gotnlbqyj.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gdwdtgezy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ggpgkvmdn.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gfqertwcr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gtmsudtzi.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/guslvpwcb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhpsuto.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggkoukmqg.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gemebwsni.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gdcgjtbro.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmkxztyix.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqjklnonz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gozdrgrnb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gijtbzcdx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gydptotut.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/guzuzloxj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gvxvwbmwi.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gpjmrcsdz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gznjcoiog.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gdpvdgpaq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gkbnwvoak.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gxqbcexuk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gxzmfnmca.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gqfbqinex.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gxvklpnqc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gxdupintc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gklfunivd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gsdbzzsyq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gboudnciz.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gichpvlzd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gztapdpgm.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gctunrwdr.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdkigaxfz.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gasktqnaj.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpvxswlzv.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/guxitrrbc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/glvvcpokp.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gbwnvmgny.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/guctlczcv.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gvpvgclfo.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gosdfsggn.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjwvnqenn.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gdwuinzii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbtnmayj.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gsljykzzv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gedcirrux.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gjzunyfdu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gooyvtfkf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/grozdkeck.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gdrjtplyj.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gkxwfykqb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gkcicehvv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gxirfdcyf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzfzvojhw.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gxogpcrpb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/goltwpxxg.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/ggpotjfag.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gdzhuywjx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gwzqwoozm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gordewehi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/goskrbxtr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gidiiurpp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/glxugfgqx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gqigngwqu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gjcxbmqos.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gqjyqucea.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gwpwivqrx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gaucsvefw.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gxzcqhzzr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbozenvjm.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gkafwmgjx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gzdkmqwea.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gqhufvgtj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gskzxzjrh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gpdrgdjgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gzfbvlgue.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/giqrxmxdo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gqlfssizg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ggjdkucyr.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gqyvvedqa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gghtjisvq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gnibkegal.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grmgakdhh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gnmwyhted.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gjsflqjax.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gjpcyoeti.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gnlixpemm.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gqtkctgmq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gcpkdhiyv.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gzhxdupdz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gjwikdcgb.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gtconeueu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gjvtkvdvt.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gqlfykzjg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gjrqtfjme.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/giwgmdlmc.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/glgolqizg.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gdidrkfcu.sHtML


<!-- 参考信息 -->