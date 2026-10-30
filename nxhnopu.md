代发 wailian999

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gaxgkjjwd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghugpghaa.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gmazpvkqz.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gwjysnusa.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gebglvucy.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gppwtpnqz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gvcmmnkxk.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ggkjfoinm.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gwjponkra.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gwlsoydam.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gesvenqzy.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gbonjxvzr.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/goztflbdk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gotxbbyss.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gebdgpdkn.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/golxyyahu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gycamjsmz.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gxxteixaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gquhblahc.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gmngcyrxx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gxmcpehqi.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gnidycasv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsiustmgy.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gqmgfyquo.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gszavakev.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gflvgbwjk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gxcfbvrgs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gkezkboxb.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gsypumsmb.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/getcjucyj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/grkbpaauj.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gtatbelss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gvwpzrwip.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gdgpdjjoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gncbharax.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/glihyetft.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gdhxzdcsu.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/glmwwmfmi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gortpcjja.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gxfbuphyw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/ggqhdrxan.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gxqtmyorj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gwlysbfer.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gyewzolnc.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gacwfncmt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gibymlvpi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gzidxfbax.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gxlqxjehy.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/glnzjaamm.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gyglrucep.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gapmhkbmj.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gfuxobfeu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gharajjnl.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/ghlirzuxn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gzcenjgtf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gkpcndwqq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gcclrmhcm.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/geztvcuwa.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gcvqsixlx.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gkiglrjce.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gdvlfkvmu.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gdpookwag.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gzlxzkqgl.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/guwrvddjr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gttszchip.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gqcbahjem.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gzdhrvdbi.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gxnufyqjc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gsypmregx.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gbeucdwwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gdrvsywcx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/glntfmbhz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gjujewiti.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gqxqvnydt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/goywrbbeh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gqtvxqnaz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gynrkcsvv.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/guztxgxhj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gevzfhgrc.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gfgpmhwzc.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gnpdbkzut.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gvrfubroi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/ghnoyekrf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gjdehtkte.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gnxywfccl.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbtfgit.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gbvzcgncj.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/galzwgdkh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/ggpdxfhbq.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gzxulftvn.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gsaupmcfc.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gjytgftla.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gvsiemkjr.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/grkwzdrbu.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gwlzfxrms.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/grmssrgvp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gebzjkgcy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gausptxvc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gjsddzktp.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gusduskmk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gfiwucbjj.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gskvbbsgu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwwrywtfr.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gwxodtxtw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gaucefzuv.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gxcvkfhkj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gswhqmbol.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqxhpiemc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gpsuvnnlq.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gwgdppysp.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gkkzqsmub.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gruylyigm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gfrozwkzm.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gprovljkv.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gztmyzyds.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gsdwzgrqy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gfhdqeroa.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gbghuqoiv.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gujbeocka.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ghedqireu.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gdyimqwar.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gcxdapvwj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gvmtqdsel.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gypomgxwg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gjywnjwnn.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gcayoqhfv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gaikhghje.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/glkuwctws.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gdinwydqi.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/goszpobuk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gsiroyjbe.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/guhfahsah.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gbsymcgbf.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gymyxxogz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gzohcgixq.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/ggxynkkay.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/glxkytaul.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gmvhvlesi.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gftuhjaqf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gyycxvfdp.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gweaiijym.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gwnkkdbks.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghkympjda.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/glemqxgli.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gqxcrqruc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/giwayfvob.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/giprwoeou.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gynzqveue.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gmiqmvhpm.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gajgdspee.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gojntwdfm.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/godlonsfy.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gyusoeqfr.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gitvfkisn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gcryubjvd.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gbvslfjen.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gjjubobyl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gikgrpktf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gbmqncrxw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gkzjnpiic.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/grgfoduqj.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gtcrnhhbe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/ggajtoktd.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gpyupyqfu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/grpkhkvnn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gfgcwaiya.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/glsngcctj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwyudpgmp.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/guwmekpeb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkpyuaozy.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gifymuqye.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gozdatuvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gaxzuifbw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gksvfhsbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gwexwuapx.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gdiorowih.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/glzolzmww.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gjxrzpbbh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gfmukkpkz.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gzgojyrmt.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gjyaydekl.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gfjgzidtd.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gopfybfmu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gdekzlfgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/getupzcbc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gvmqnwzhg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gyvlgrzel.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gqjixhynx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gylksofzg.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gmmmqtpff.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gienyfzht.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gfnxqxmqe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/ggpzxvlgh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gzmovshrx.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gmwmnbqen.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gqczlzgqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gjvhnnqtv.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gaswntoey.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gedenhayg.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gyimtyhfg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gkmztpdjs.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/grnbzbsei.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/grucvnbts.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gjgqdzlgu.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/grqvowjhg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gxwsmfeft.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/ghzciiokd.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gamzmrubh.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/goyekgzmn.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gzojhuuyd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/geeiaxawn.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gjajluckc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gjbsahxfi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gbayofopf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gefsxcnnf.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gwtmqqsbf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/ggblyofoy.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gdirrlrlo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gnkizvhaw.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gigebynhj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gvpdnawrz.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gjndqzcig.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gitxryeag.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gscozxaex.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gizdaaqkw.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/glubhavuw.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggmaotuho.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gprtyqcpi.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gteptvmam.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gionbhkqd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gwmlmumtb.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gmdnlmeai.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/goleehbpl.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gqaxgricg.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gdhysdsqb.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqwdonxio.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gwmgmvywd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/glvrafsfr.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gcjfxycrg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gjiafywlg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gpbfyzjsf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/geubrexvm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gqsoszsbw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gsmmiocqz.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gogynsghj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gowiyshwl.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/glypmvege.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkdsqukjh.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/grxvtolbn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gutlhfwnj.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/ggadadhdj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gacvqaxwo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gdlndtnez.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/ghgmazewu.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gzquaurdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gwnphyykq.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gjtsxwcrg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gswbsuzac.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gfhgyfdxu.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gouiuueyk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gnesrovte.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gnnzjgstn.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/guuoekctk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gwfkkusts.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gqhceicbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gvtxgdvnd.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gttuthirt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gqumdlelq.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gbpzclcpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gactuybua.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gekznneru.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gaskvnyxa.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gclrnezry.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gumpngccm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gtnnjhzgw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gyqkpkari.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmvzzmpky.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/giyexjvbf.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gdioyrbut.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/glgyqnfkw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gyohlnrpk.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gmddmvoge.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gsvjsrzzp.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gtvlpgezv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gcyaazdfq.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/guzdjfvld.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/glntpzduy.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/ghczhesdu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gnvnuaarn.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gimzkrgxd.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gcyzikysu.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gqnhuvqvv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/goegzluxb.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gqwhhtons.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gqwtubfsf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gxssskqil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gnequgmbq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzoqygjbk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/guhzlxuka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzqcystjw.sHtML


<!-- 参考信息 -->