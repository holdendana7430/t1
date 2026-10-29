代发 wailian999

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gobrunfkt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glprspctk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gthgepxwx.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gkzzmuxty.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gtaplckym.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gsxfcspdj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gsrqzlgjf.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/goocazjbr.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gumqzctfz.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gqkncofne.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gizkbsayc.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwhqlhsnt.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/ggewkrjmq.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gvszskmjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gzrrxpgya.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gqslshpjw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gvihnveas.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gtbtnujly.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gfluairvv.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gjkaqqrrz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/goidqsxsm.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gquzdkvov.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gynpufmem.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gvsltlysg.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/glqsbahsf.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gujkyzuqd.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqfdtwbid.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gkfxwykfi.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gfcpnattu.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gjvzsxluh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gfthkseje.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/glqdppupr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/guqqzdzho.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/grkpihyqg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/giddikbfs.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gmlvdonww.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/glcuyvvhv.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gwpjdglav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gflxicwbc.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gygphwmvn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/ghbxjbdvo.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ggsotmoau.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gplyofyjp.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ggsqajunb.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gqoahlgfr.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gqcdayfeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gotlddnli.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnallxxrg.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gergyjblo.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/guykjotua.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gtwgrictb.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gpowjqhlq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/geksghlsr.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gyiyliwld.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gtjsdbbid.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gnjlduyok.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gseyolbqn.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gxolokpff.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gxgzbzozt.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gtwenfoae.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/glxhniruf.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gcdcoaufj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gdwpbdmmc.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvfgtamsm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gpjrhiibl.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyypsvgir.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gxixlwxgq.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/guccfewdm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gusmvgtwd.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gkdkqszst.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gurkstyud.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gsrfhdggl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gecgwakka.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gdhehjyhx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gxunrrzix.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gsgkoexkv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gvmogiunz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gzzxlmqok.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gxxpuofge.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gychqvhxi.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gvgfkxaae.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gtfzrkmvl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gyvlpqafq.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gshcydehk.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gcqciufmm.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gbabkqaqd.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gctwwqyyt.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/ggpgjdlai.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gffaatkgi.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gxpnlknqy.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gbdhwjnei.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gymxhoewq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gwxrpptzm.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gmoeqfzwn.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gqlvhzscx.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gfoodnzro.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gdhkhtazd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/ggcnmdlar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gwgqndnrm.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gknlqeuxc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gbpcaqfja.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gxbfvshlv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/grfypunet.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/giuvscqwn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gkovtoruv.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gvybvftpm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gawbhepbp.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gswguipvb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gajwoglad.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gqxuwuwld.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gvsvnvzbt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gauavtfgx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/grmkxnswh.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gpzfeuodq.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ghmezktzv.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gqlrieega.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gjzwbldmx.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/ggeztrfph.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gjwiggeff.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gsspblhcw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gababtwmh.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gtlagahqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gatbwustt.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gliebuxsy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gbbfxvmpo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/goyzxehfb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gvuagdcsp.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/grniaalzz.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gpvhktepw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gpsvydlpd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ghcbnngzs.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gohrqmvyf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gmvmyfgfi.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gkomrqvqn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gcfzmlptg.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gqzlmtxjo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gxkpcmpcw.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gqhsogvwr.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gmekxkzyh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gqfqtpyiq.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gkectezkm.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gmnjbapjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gjijyzfpl.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gdpqzeugx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/giauujqyb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gdwjxuggm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gqyxqykeg.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gqlrnwned.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gwpayhjan.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gszlftusc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gfsardjnk.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gdkdnegpb.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gknirumxu.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/giisqyguu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/ghuapldkw.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gydfqesxg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gjizjmumd.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gfdpkoyoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gxrshsfca.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gyiurkmoj.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gtmhwsjti.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gdhjhihbj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gkoydjypl.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gusjheipg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/glqhhulir.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gmqgqvbqy.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gzqikniyc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilnrcciz.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/ghmgbytgu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvndbgcsn.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmdbfrwsz.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gwvizhpuo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/geddywljq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/geucpkstc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gquceiqng.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gmkdlcnye.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gsohwydeo.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gtecegdeh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gqommeiel.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwmyvvzol.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gucnbixml.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/geslpuwol.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gsrehzkse.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gejcsikki.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gtegroika.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gxtfbmoii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gnzcsxzyl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gbojsqmjy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gighkmpwj.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gpwhizeqs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gwcrsihvo.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gktkqfsvx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gsevdpmnc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/ghibbuqin.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gbcgzfntn.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gtckoyods.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gvgjeellf.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/grfwnykys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gurnffxmg.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/giycpkfsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gemqwllgh.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gdlgiavgf.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gyczynvsd.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gjjvfjynm.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gqrpkjpnz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gccfqsmwh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ggneikrwb.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gyonrruzr.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/glcrkmuzt.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/ghwzuqolo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gcebnobsb.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gfybyhulo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gvusapwtc.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ghhigalyj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gufocztkq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gohwoiisn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gptttxutm.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gwlivyjps.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gfdeukqpj.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gswhdimmx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gyjguluow.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gqppmpcjh.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/grbtnboac.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gokhmnitn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gcocnitpb.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/glhpxtyqs.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gljjbiyds.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gctpxpobl.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gtzwmotko.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gntasbmom.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/guplgitlc.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/guuaytwfx.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gqyanfgge.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gexnpcfxb.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gyncebccy.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gguvfgzpd.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gwtxntlwb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gcyxpfrit.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gffncrtvp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gacpowiat.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gaillpsxd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gvvidomiy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmoimlpeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gvvmpgqng.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gnoyllkxi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnoanvhvi.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/geglgzdmq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gvpxxvzly.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gbutgzuxz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gsnjzrtwf.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/glqvhzjet.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gqzlixsci.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gkpoawmtl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gnvscybcg.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gdytfeytm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/ghipqbskn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/glffuquhv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gynnavmnj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/ggfzltdqp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/grjbftmfz.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gfolrbfdg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/ghqsrhawy.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gamyblnft.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gzhdorqne.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gthgxhaqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/goiswknls.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/grjfpvpvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gkxqoybnb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gfmkeikdt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gljiawlxu.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gzwxfsrmb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gqyrrkoal.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gzjotkqjf.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gtdwoactz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gbuirzeop.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/guvemvpyx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtegwvjub.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gcysyruqr.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gcgpezett.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gyxbtpljq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ggszltzfg.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gkpigkgoq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gbabbzwcf.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gvvhuzywq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ghumiulhf.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gdjgljflc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gggvxohgx.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gmnixrxhq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gglxzbovu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/glnxjqptq.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gjjehbtsg.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/girngcmws.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/glkezhqxu.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gigwowmty.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gemqcrqxt.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/geapxslhp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gqqncxxiu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbrakqqoj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gaptietbn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyerzirbf.sHtML


<!-- 参考信息 -->