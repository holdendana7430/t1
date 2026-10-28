代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ivvv.top/gtqmtgbqbk.html

[Q90] 生成序号列
来源：http://hz.c1oappe.top/gtzvsmbydq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangdashe.top/gtpzdtbrxj.html

================================================================================
来源：http://hz.yueranfly.top/gtudifjuaq.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtpvcxngwn.html

================================================================================
来源：http://hz.yj20258.top/gtcelxkgry.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtzpivuasy.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtvpwypuui.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gtcjsldwdx.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtjfxlbgis.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtifhrdgnv.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtcpufyflm.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtbwlyzrxx.html

[R04] 位置参数
来源：http://hz.guowangkeji.top/gtgceairmv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hammf.cn/gtngixebzg.html

[R05] 参数默认值
来源：http://hz.dianchejie.cn/gtmekvigba.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtcnhsiuaa.html

[R06] 判断命令是否存在
来源：http://hz.cashguo.top/gtnlpmvifb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtcznsenol.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtxhyulfen.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinghuilouyu.cn/gtffoqkaev.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtwjkcnbth.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtsyvjnwop.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtuapgylfv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.mhx1999.top/gtqoeayfug.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtgcgkggdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtbxerltdu.html

[R11] case 多分支
来源：http://hz.yuanzhike.top/gtoervkkqd.html

case "$1" in
来源：http://hz.shzxlz.cn/gtmcymeort.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtkljllujd.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtszxedgkn.html

*)     echo "未知命令" ;;
来源：http://hz.kuanghao11.cn/gtwfxrjagy.html

esac
来源：http://hz.cashguo.top/gtpdzplhfo.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtgslbzczx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gthnooalfe.html

[R13] for 计数循环
来源：http://hz.ywan-chungtsiang.top/gtxwdivrvz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtegqzeqbg.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtezwlwtnz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtxsbymhfi.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtbxktetrg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.9152youxi.cn/gtrfskawvm.html

[R16] until 等待条件
来源：http://hz.shuidangran.top/gttfrcysie.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtlzxocfqc.html

[R17] 数组定义与取值
来源：http://hz.snrcjt.cn/gtcogwuayg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jiagoushi.top/gtmpavrxxc.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gttxuyzpyp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtdexabkae.html

[R19] 数组长度
来源：http://hz.smart0.xyz/gtrsrmzhey.html

echo "${#arr[@]}"
来源：http://hz.daria6918.cn/gtwcsurxup.html

[R20] 关联数组（字典）
来源：http://hz.jiagoushi.top/gtiyjtfcxn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigufen.top/gteqtvleyk.html

[R21] 字符串长度
来源：http://hz.tian-w.cn/gtblibvjlg.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtdonmcngh.html

[R22] 截取子串
来源：http://hz.meibo888.top/gtiimscede.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangtech.top/gtlpsptoso.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtptiyuhxr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yangfankeji.com/gtjojvoasp.html

[R24] 大小写转换
来源：http://hz.wangshuangyany.cn/gthmuyfrqu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtpuxpglfx.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtfezbbeed.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gotoacloud.top/gtchezhloj.html

[R26] 命令替换
来源：http://hz.ydjk.org.cn/gtnorpbetw.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtmograedp.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtouxtwyke.html

echo $((1 + 2 * 3))
来源：http://hz.snrcjt.cn/gtucpnfbvz.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtvxwttptl.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtetajxuvs.html

[R29] 定义函数
来源：http://hz.ydjk.org.cn/gtjvrvvtjx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gthtqtxnpa.html

[R30] 函数返回状态码
来源：http://hz.tianlin.xyz/gtbyxbpwwv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtnnbfpmls.html

[R31] 局部变量
来源：http://hz.sysykeji.top/gtbjxweqgs.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtssutuomm.html

[R32] 参数个数校验
来源：http://hz.jqgufenzy.top/gtaosglqvy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtjgljmspx.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtvamqfuhr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtrkiyyggv.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtlviqrfbh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gthpvyrkzh.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtbmixqtku.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fengsongda.top/gtzdoewysq.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtsqzivfkp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtbkqgxzrj.html

[R37] 把输出赋给变量
来源：http://hz.xuetiantiany.cn/gtredcukdh.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtebzjpnbt.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtismflklw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gtdfafiipv.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtnwgmwquw.html

cmd > out.log 2>&1
来源：http://hz.quarkkingdee.top/gtvmqqbipr.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtwwawgndi.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtvktqhxer.html

[R41] 丢弃输出
来源：http://hz.jyoumei.cn/gtetmksygd.html

cmd >/dev/null 2>&1
来源：http://hz.yj202588.top/gtiwgnglyp.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gtatmsgrng.html

wc -l < a.txt
来源：http://hz.zycfv.cn/gttdseddmu.html

[R43] 按名字查找文件
来源：http://hz.dashuyun.cn/gtpjwywodw.html

find . -name "*.log" -type f
来源：http://hz.fzhhl.top/gtqrudjkzx.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtztlfkoty.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gtgykiaumz.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtftljeisj.html

find . -name "*.tmp" -delete
来源：http://hz.hongshengwenyu.top/gtxgwpnxhi.html

[R46] 递归替换文件内容
来源：http://hz.bjfxy.top/gttzgnerkd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.9152youxi.cn/gtgvytawbr.html

[R47] sed 单行替换
来源：http://hz.jinqigfzy.top/gtzkuvqmqw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtvgrfoyqd.html

[R48] awk 取指定列
来源：http://hz.yanxiufei.cn/gtdrjdwvxp.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gttcwgfnlk.html

[R49] awk 带条件
来源：http://hz.cqqwz.cn/gtaioufnbl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtgjaiihqc.html

[R50] awk 求和
来源：http://hz.hywenlv.cn/gtguthwdop.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gtbxcoeszj.html

[R51] 排序去重取前几
来源：http://hz.quarkkingdee.top/gtxkmbhwyf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258.top/gtxuffmigh.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtfedroaqy.html

wc -l a.txt
来源：http://hz.yj20258.top/gtkgbapcjq.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258888.top/gtqvmvtaud.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtkmfmtpas.html

[R54] 比较两个文件
来源：http://hz.jianghu66.top/gtewczzhml.html

diff a.txt b.txt
来源：http://hz.tianlin.xyz/gtkxthatwn.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtsmxitiwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtrzcrtipl.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtdntytwwv.html

scp file user@host:/path/
来源：http://hz.mhx1999.top/gtwbdyhuth.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtkvqepyae.html

ssh user@host 'uptime'
来源：http://hz.redwolf501.top/gtxkgmrstb.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtuulkbjob.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtgrtvspdi.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtuntovfst.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xinyue.icu/gtyzhoshyd.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtjnyoopnz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtdfjsttah.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtmmbgxrgr.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtegimvxwi.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtldxsyygg.html

du -ah . | sort -rh | head -10
来源：http://hz.tianlin.xyz/gtdgqxpmus.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtsjeaypsg.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtslbedhwk.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtccrsusbm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtigbpmqkq.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtgpxkfutr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dashuyun.cn/gtkwvmdkzb.html

[R66] 定时任务
来源：http://hz.zhijiandao.cn/gtnjslaavb.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtsocyjmlr.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtsngqcxix.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gtkagwkiwx.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gtgeusejvt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinghuilouyu.cn/gtlphlkxsp.html

[R69] 生成随机密码
来源：http://hz.gogol.net.cn/gthydslzwp.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gturwihxln.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtucokbyyw.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtwimwfala.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtjypbsoeu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj202588.top/gtcxwwmpvp.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtuzeflqrt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gticwldkkn.html

[R73] 分割大日志
来源：http://hz.jiagoushi.top/gtewowyxfm.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gtuctonzvv.html

[R74] 批量重命名
来源：http://hz.ivvv.top/gtuvizspsp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gzhubu.top/gtrkbvifpd.html

[R75] 导出环境变量
来源：http://hz.aizwys.cn/gthyakrroh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtefwbygyr.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtrpkrsdnj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gteqqfyhga.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtqfflnfap.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtmmooqqbc.html

[R78] 交互式菜单
来源：http://hz.hongshengwenyu.top/gtupideilo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangshuangyany.cn/gtoiggpeqd.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtpbraiawu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gaohongyu789.top/gtyvdgskca.html

[R80] 查看脚本执行耗时
来源：http://hz.cucudq.cn/gtlwklivxe.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtbpwlxfnm.html

================================================================================
来源：http://hz.birdmap.top/gtoogddkml.html

S. C / C++ 专题
来源：http://hz.zhongyouzk.top/gtmcmkwjlb.html

================================================================================
来源：http://hz.jiagoushi.top/gtkmepmrog.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gthhpuvqqu.html

#include <stdio.h>
来源：http://hz.chenzaomai.com/gtbdxrfypy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jyoumei.cn/gtcyifdgyw.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtipcgawgo.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gttjidmkpv.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtctznzrgd.html

int x; scanf("%d", &x);
来源：http://hz.yj20258.top/gtoihuizee.html

[S04] C：字符串复制
来源：http://hz.bjfxy.top/gtomblncof.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtypdzcvco.html

[S05] C：字符串长度
来源：http://hz.jiagoushi.top/gtzuutbksf.html

strlen(s)
来源：http://hz.sweek.top/gtiubvmdve.html

[S06] C：字符串比较
来源：http://hz.hongshengwenyu.top/gtqkvyfjtz.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtrvnmqjci.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gtiodvpybg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhijiandao.cn/gtnjbjdjeu.html

[S08] C：动态内存分配与释放
来源：http://hz.ehwqpu.com/gttdbtgjca.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtxossiaia.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gtsvlocivh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhijiandao.cn/gtbzeeonzo.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtorwnljfa.html

int *p = &a;  *p = 5;
来源：http://hz.quarkkingdee.top/gtxevftqlp.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtvpejeyvv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zdqjudy.top/gtfdazeoqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.kuanghao11.cn/gtnntdrjgc.html

fclose(f);
来源：http://hz.cashguo.top/gtyxkvlacz.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtegpoyden.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtijlaeulb.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gtktbebuma.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtbkjasqns.html

[S14] C：枚举
来源：http://hz.yvedp.cn/gtghqrwsct.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dashuyun.cn/gtqcaixqob.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtbxolcsbx.html

(double) a / b
来源：http://hz.jiagoushi.top/gtspyqpkgf.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gtvfygzacm.html

x |= (1 << 3);
来源：http://hz.redwolf501.top/gtlkydseln.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtarrbcyet.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtrebobvsb.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtzhtkbetn.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtgzqlvvqm.html

[S19] C：快速排序
来源：http://hz.jianghu66.top/gtasfzewsn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtxoowqnia.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtxprzqzga.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtvxfmoaga.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtzejkhbbl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtzpdmaoya.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtyflobcxo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtygkmachf.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtbsnsbpwq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gtfzfuwalj.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtydjbrojf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gttfxzixub.html

[S25] C：内存拷贝
来源：http://hz.wangshuangyany.cn/gtwxukkdvb.html

memcpy(dst, src, n);
来源：http://hz.dianchejie.cn/gtehyxainl.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gthaduiyln.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtaqgprdxf.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtuironyuw.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtjwjjywic.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtsadqujpi.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtfbhpmwsj.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtfgxywrzr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shangyingyoupin.top/gtychxfplr.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtlvzjhivv.html

#ifndef X_H
来源：http://hz.yueranfly.top/gtzsllwkmr.html

#define X_H
来源：http://hz.gaohongyu789.top/gtxpclnrse.html

#endif
来源：http://hz.zdqjudy.top/gtwsxzmtyv.html

[S31] C++：Hello World
来源：http://hz.ydjk.org.cn/gtqsptnjkw.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtddkswwll.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtdasdpldv.html

[S32] C++：字符串
来源：http://hz.aizwys.cn/gtdrflcuvj.html

std::string s = "hi";  s += "!";
来源：http://hz.birdmap.top/gtemxbbadz.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gthdvbxmke.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.quarkkingdee.top/gtrqwylnhy.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtfsawmgpj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtfoomqnww.html

[S35] C++：map
来源：http://hz.tanke756.top/gttkucuhiv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtotdlpkbp.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtkoapajvb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gthvtvvajm.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtnkonhhdg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jyoumei.cn/gtxkboivzs.html

[S38] C++：排序
来源：http://hz.xziqi.cn/gtbagwsqma.html

std::sort(v.begin(), v.end());
来源：http://hz.shangyingyoupin.top/gthxnqlwzy.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtlklzlmqg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sweek.top/gtuksysalp.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtkxiawehm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtjwytxilo.html

[S41] C++：类与构造函数
来源：http://hz.wangdashe.top/gtrwymocci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangdashe.top/gtabvftiyh.html

[S42] C++：继承与虚函数
来源：http://hz.jinqigufen.top/gtuwecesip.html

class B : public Base { public: void f() override {} };
来源：http://hz.xingfuxueyuan.xyz/gtqusotfwu.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtjxbdmoew.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtpgycknuq.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtklruewiq.html

void inc(int &x) { ++x; }
来源：http://hz.gzhubu.top/gtvkuynhkm.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtaluiupne.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtguvildtu.html

[S46] C++：函数模板
来源：http://hz.svipenyu.cn/gtwpjozeto.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yueranfly.top/gtakcmrgst.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtehhibzcg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gthtznqbcq.html

[S48] C++：逐行读文件
来源：http://hz.haohaochexian.top/gtwveiccnh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtdmgktaji.html

while (std::getline(in, line)) { }
来源：http://hz.sufxvd.cn/gtfzdcwtkt.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtvdnrvbii.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gzhubu.top/gthnerssvg.html

[S50] C++：格式化数字
来源：http://hz.xylfe.cn/gtaqwejvkf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtvkvbrkbr.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtevbvlynn.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtvwnmkryc.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtyrdbpzhr.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtsgofjoky.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtorolzayy.html

std::vector<int> w = std::move(v);
来源：http://hz.guowangkeji.top/gtwmxlzzcz.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtjdwenkrr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtydqrqbfb.html

[S55] C++：结构化绑定
来源：http://hz.zdqjudy.top/gtkhrlsbsr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtppxdfvzs.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gthqqtvczg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtzhgitmys.html

[S57] C++：编译期常量
来源：http://hz.yuxming.cn/gtemhhzhsy.html

constexpr int N = 10;
来源：http://hz.zhaomingkeji.xyz/gtthijxzcv.html

[S58] C++：命名空间
来源：http://hz.yj202588.top/gtljkooean.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtirnhmvzl.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtvdacvxps.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtgosxudfd.html

[S60] C++：遍历并删除元素
来源：http://hz.dianchejie.cn/gtkmgsikqp.html


<!-- 参考信息 -->