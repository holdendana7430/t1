代发 wailian999

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/goqhbylqe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaadxtmcv.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gwrumimbg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gnzxlaiqg.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gumrictwx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gymwqpobq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gwjeuojsy.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gmbecdozr.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gaoaglihg.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gwxdshdfs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gzfxpmsvv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gtdzpksph.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gzzxtdlzj.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gwjqdshxn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gmljnovnx.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/glrjivusn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/ghjqoqdia.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gywvcomcq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/govdiougf.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gogetolof.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gqmghbocz.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gsilzuwnf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gwkjqyvtg.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/geglyfhcm.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gehitmgou.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggyjyobwx.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gxqxfamgh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gylnfpggo.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/glcizspff.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gnfvvybgn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gacheprvg.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gnhcbqubd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gphvanevh.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gulweffix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gfabfcanz.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnimjhiyi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/ghjwpzosz.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gzpxcjhal.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gstrhtilv.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdnnjqclj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/giroxzlrh.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gikgangqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gllmjuzri.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gnbgslqsc.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gwuytgicy.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/girxjqiki.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbwcdsknt.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gbdzzvugb.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/ggfeudrtu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gucrbewne.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gupdfkhzn.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gmesmczxw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gcrkljxya.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gwctgediv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gdmskwijo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/ghokoglsd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gdnfqsfpk.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/glnbpesct.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gddbjselc.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/ghxxlksua.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/glzddkmnj.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/ggkxyqoii.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gyhakpqgu.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gxtpzcjev.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gkoymmyru.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/ghtytqikh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gbucngepf.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gxhsojnpr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gqofrscnp.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ghlkqnzdz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdnccpf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/ghzfcfjne.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gypfdneyn.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gctuxqqtt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gstbluslq.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gaufozwdw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gbjpxzfmr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gsrtztabe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gqgexlkre.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gwjlwmazo.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gffuuuzhz.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gaposqrsp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gvkzlhsvw.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gcloccifg.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gczyheqha.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gracaglxg.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gtiirnsri.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/ggmmpnmwa.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gxbnpvwaz.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/galskqfjs.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gpacjsacu.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gaxvoejge.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gcznapheo.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gcwrnqygm.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gpffomywo.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gqitwhfab.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/glbcchmpj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gwsqlliqh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gqgdkhcvf.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gmycwutgu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gkwkvlzol.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gizxzcqhr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/grnybkbvj.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ggudjvqlp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gajrflohf.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gvaogowiw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ggyamqgtz.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/ggklofmdl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/glkfhlovw.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gqakimpwt.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gyuzamhew.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gggsgoehy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gumqbuqdx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gmbwlgpzt.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/ghpziyeun.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gttezmbrd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gktprojvy.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gcwozfsge.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gzmhfszcb.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/guhxhdrxp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gxghcxdgb.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gslxonupn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gxzowpomk.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gmplyfzfp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gzwvgvogs.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gjzltsqso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gcwanlmqk.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gpmwvadtw.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gwhumylie.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gondevspk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gbdcuehsn.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gqygydzlt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gbnwwdlcx.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/ghjwgjybm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gyadtehqb.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/grwoupwzy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gxjhiaekb.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gjjvujdcc.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gqobbzlqi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gtnamtzdw.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gydamfuwh.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gunrprzhl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhtknqk.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gfrwuypyq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gbnfhxful.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gjcjjqdsw.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gciaryeiy.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghgwnlcup.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gurnityfw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/glezixalz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/ggqpwxzqm.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/guxlddnbe.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gyagqxgql.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gkohfrpnl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gwmbxklxz.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/grjplhefz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/ggmvftooi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsngiikca.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gohwhsozb.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdqsxagpr.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gjnyqtvkz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gfidwjdls.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gaynarcfv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gyrzjdqkt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gubpmyhft.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/ghbtsctkj.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gkvkbygfa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqylbetgu.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gubladufw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guohildxd.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsmjekqrr.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gzysvqkyv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/galxaeive.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gduexnjyh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gndjndznq.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gxxutgvwn.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/grkexwhmm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gclhiqsvu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gxqhujelr.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gspcrliwo.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gafuzcgpi.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gelryyjfz.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gjsyfgyeg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gyhalucnp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gyoobnhgo.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gmgxsscqj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gjzzqmkqr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gqqigwqwm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/giqdqkhyj.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gnufpjdlx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gyymdxmte.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfrwgjcef.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gixwmjazq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gceaaceet.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gfoiilolp.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gpybdsaxe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gmaiaixqc.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gqkpjemvl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/goeewihuh.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gqojwxjaq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gjoivbjgf.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gbxvbmset.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gwtushyur.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gpnhzzbiu.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/galixzvil.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/geudzzyak.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gvoogpdqp.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gmefisenw.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/goeeptgia.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gqtwnyjtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpzgermfl.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gkbkydjaj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gzpvgtzdj.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gfvpsjqkf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gahqaddjr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/garoblrng.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gksfrhdxd.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmjvkfmkl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gzbftamik.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gkbcavexm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gylfgqcsn.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gmlqqbxrh.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/ghqownkbt.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/ggvsoucpy.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gtbijjwlv.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gwiqhifio.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyusdyeeq.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gnaranmzh.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gvyfvkclw.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gpinrqwko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gytbwlqdl.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gzvbjmdhq.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gmtwbldtm.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gglikujsq.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gxnvutzxj.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjnizdkar.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/ghsponmgu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gdmuqvsas.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/ghrdznfbx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gldwyqkqd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxmhjag.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gzqyygzqn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/ginvoemzz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmiilwydf.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/grzcmpaog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gqxuvsknn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ggrmwzhkc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gpseexwlf.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gvycwmlpw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gzimwvufa.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gkxhridsf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gjdirqquf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gdcpusjpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gzwhsfgnh.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gkknykmzq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gnvybuqod.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gbhfqbili.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/glyetljgi.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gxlijplfr.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gtxxtsgfh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gclsgooei.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gyddmsoki.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gxtiepqbz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gmrnlzrtf.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/ghlzaoqoi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gvhrcugia.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gmffjsdfl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gdhuldwhi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gzzieptzn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gtyrxsmkk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ghnmlzhcb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gzrvcrnfi.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gevutgslu.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggleyrcpw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gvgjsoxga.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gvuygtgtq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmneooyvn.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gcanswvvj.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gcfreqvko.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gmmirweqm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gqalmemnc.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gygcxjfzb.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gabnvfjke.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gxwpqwmwu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gmfpxjiox.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gjdoyaizf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkwejfcgc.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/glcrbmsyu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/ganqueiua.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gfkveieqs.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/govgoycjj.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gtlddypfe.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gfxtwckgh.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gumrrmujt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gkppinwtm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gyounlqvw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gledrobps.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcmjnxdus.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gadfcvxxj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvwgllwjo.sHtML


<!-- 参考信息 -->