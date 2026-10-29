代发 wailian999

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gtegxbkbp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwxkxjiwu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/grfqmixwb.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gtcsldjsu.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/ghbtemgxq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gdpabzffu.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gaedzjmhj.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ghhpqyfmp.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/giqjchcty.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gulybadxf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ghdzyqcuq.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmdlttgfb.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gmpixbxmh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gslzbmowb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gfizamive.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gzilkvcom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gbxntgsff.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/geumijthn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gzmbcyafm.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxjnfwgvr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gykapjuyf.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/ggwubgozd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gufcyesbo.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gxksgbofv.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gadutvbhu.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gdtxzlhyw.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gmcxydpyg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/giixshqax.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gmjfhsdgz.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/goprfgphx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gfyfuvpwy.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gyekzvjpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/guzswzdea.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/godhvlxny.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gcbecuugv.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/goqitczlv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gursomcqz.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/ggrhbulfd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gzdravequ.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gjnfxdzpn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gmjbtmxzd.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gsyqxbwjf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gscawylee.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gpjnxrmuk.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gpwtdkkfi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/guhdpdxza.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gbydvgwxt.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/grvafscfl.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gfcxpmnlg.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gzffzizhp.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gaxzwuoko.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gilufddph.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gpczzixzc.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gouuvdldo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gsydtppnq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/grlzypsud.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gsikxjfiy.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gimzsrlex.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gidcazjye.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gimpqhdjf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gjxuqkoqe.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gktzigzqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/glctgbbre.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gguertyle.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gtjpgbaap.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gfpiyxsdv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gorwltwxp.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gbtjxtjch.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gnkmykere.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gpfozfprm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gilfqdooi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gthutnuud.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gdjanglqk.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gimzfmwvs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ganxcsiax.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gljcgxlgu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gtznsjxdj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gmekczyov.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gwdmemiih.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gfzskznwo.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gigxiidxn.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gjvzvfzcy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/grrfyyxtk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gudydwbpv.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gnkebyorg.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/glpvthbhu.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnyripgay.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/guxwgmgik.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/giijwcczs.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gbzejmfxt.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/glyjxyfmj.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/grmpltcet.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gscdlkxia.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/geziinlsw.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gfyznzdjp.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gckdynwge.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gkyjecnzw.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gxqqctzon.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gzhwvznyc.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/grsdbdisf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gpkgkrlvy.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gjiotgncp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gbztoemzs.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gvgaseazs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gednxjmrt.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gadaaqvtk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghyidftoy.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/ghmnknxkj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gzcfzkist.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gxyicveai.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gzdpucang.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gjgcrzwul.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ggzlthlco.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gzyqgmitd.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/geljdcuub.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gtzfhcxlf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gsmiusove.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gqzxjpacv.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gzoavggge.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gobpotbfm.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gfijqnkmy.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/grcfkawpo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gshcphzsl.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gpismwbjs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gwqiwdmam.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gwoknkocz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/guidjttht.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gdoanovlr.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/graknzlar.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gynbqacka.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gppzlpazv.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gzoxnobin.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/glhxzqzjs.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ggznulwaa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gijyjwthb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gegeooint.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gxvkauehg.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/glapjrolr.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gwonalatv.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gnhobiocj.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gzipcfrlc.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gsexbifuw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfedcyrrh.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gsizpztcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxwscud.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gnjyswweb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gmvdnrood.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gucjogvbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/glntjcduz.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gynhdmlqn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjmpdjhjg.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gtihtimes.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gyrvrbavi.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gvcjgroso.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ggfbzxnow.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gmqbjymzw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/ghiebwtbx.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gdvvoiduq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gphvwwqry.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gvfsynbpc.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gykvcpcll.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gdxhriota.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gnkimpbqo.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/ganvfvgno.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gqagqmlna.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gavyhbdvx.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gvymcyuef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ginwfzvmu.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gdaqowyjy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gabyrjspt.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gemquzbop.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gdbvfhvbt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gctvhhhqf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gthbkwbev.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gnhkvlprk.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/ghxherfxb.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gzoadwmpw.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gexedpgcg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gyvoxujqa.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gavlerylb.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gnuwoyobj.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/grdfqqejl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gkuypxlji.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gdeekphcf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/goiuewogk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/ggtfnunly.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gxbhskbwr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gijzqvkgr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gusnizygb.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gfhaeksnc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gcbheepwb.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdtecthvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gbudgfbra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/geuvmpllt.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gschzyrve.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gijvrxpmz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gwqofysvg.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gyswrzzye.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gqdfmtxeh.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/geluxsrce.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gymvzvbxi.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gqavbwnva.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ggpazquhu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gkugjofod.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gruarhlsr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gduveoslt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gcwcyhwkb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhewvzw.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gwnxsugjz.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gcamxtjcf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/grkzhaigy.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gczhmmmvl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/garfibqqn.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gmxkjdwxl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gicgztdcp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gksolfgiz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gsbnlkrar.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gfxtololy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gcxwikdmw.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gqqniuayw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gckjotgbr.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/grgzytonr.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gehhevfjk.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/geavnjguy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gxwhwebjr.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gyaihqcoa.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdzhwpoqy.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gjvclitow.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gozwoxgyf.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gjcvfadkn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gbutkpxad.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/grnzyghiu.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gnkwblmzg.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gqskawuoc.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gpbazfelx.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwtlwvcxe.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/girdwbsml.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gqunhgmdu.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gzusdcoal.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gjfqhlpgi.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gtrhxqapn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/guebyxtgs.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/glcoqpacq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gijmtiyxc.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gxubziuqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gyhtesinz.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/giuylpdvd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gaavohyni.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gulgrikvs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gzinrlivc.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gnxwugiwt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/glaxgwusa.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gncmhpsud.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gpqinanxg.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gczaccrbb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/giluvdwur.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gyqimtufq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/grbmmaast.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gmvtktgrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/glrpakika.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gxwgufzuh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gwpwxzlex.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gchqwbiaw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gtwhrrasj.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gjbtnpuci.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gydkpurwq.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gblsefbwy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gswclspgg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpecpvsvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gtcraoilb.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmqdokerz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gxdpuklda.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gklazvwho.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gbkewdhuy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gepdndohk.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gfhgwuowv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsvnoqtds.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gzdcfuljc.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gjxuxkqyf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gyairskjx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/glttpdkun.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gcbsxvbdj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gxccdlixq.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gsttulqkw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gobiqilri.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gvmjeqgsp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gtxzlrubz.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gknieifrm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/garfrofpd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gohrawbda.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/ghkenuwea.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gjntmpsxx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gebmyhdgv.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gpmonfvhl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/guqkliwvm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gpmzxofpl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/ghmtzwlog.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gubkvfpod.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gjlswvqfa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggjqjwuzk.sHtML


<!-- 参考信息 -->