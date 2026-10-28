代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtvttpebjl.html

[Q90] 生成序号列
来源：http://hz.xziqi.cn/gtkauuvxtr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtxlbkaasf.html

================================================================================
来源：http://hz.chenzaomai.com/gtiurepise.html

R. Bash 专题
来源：http://hz.tianlin.xyz/gtkzhrdtvh.html

================================================================================
来源：http://hz.dashuyun.cn/gttgepiowc.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gthqtitlkj.html

#!/usr/bin/env bash
来源：http://hz.cheryme.top/gtmdbgidpm.html

set -euo pipefail
来源：http://hz.jinqigufen.top/gtsapjtewj.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtrfgtgjub.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gtunddumch.html

[R03] 只读变量
来源：http://hz.yj20258.top/gtoabkcbsp.html

readonly PI=3.14
来源：http://hz.guowangkeji.top/gtvbumwiwj.html

[R04] 位置参数
来源：http://hz.jiagoushi.top/gtqjxrkcro.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sufxvd.cn/gtvewrevnv.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtrphqstix.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gtvukdyotb.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtsifhynoa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yj20258888.top/gtnmiucxlt.html

[R07] if 判断文件
来源：http://hz.daria6918.cn/gtpegonvdx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtdvqfxobd.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtkrxdudco.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydzc1.top/gtqtduuxxt.html

[R09] 字符串比较
来源：http://hz.nwbrower.top/gthuhtgmlh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shzxlz.cn/gtpslqzxrj.html

[R10] 正则匹配
来源：http://hz.cqqwz.cn/gtrqvkiinh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtmtxjvfys.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtahwnpvcg.html

case "$1" in
来源：http://hz.shangyingyoupin.top/gtvdgymjex.html

start) echo "启动" ;;
来源：http://hz.jinghuilouyu.cn/gthikrmfkj.html

stop)  echo "停止" ;;
来源：http://hz.gotoacloud.top/gtrsuzcxsk.html

*)     echo "未知命令" ;;
来源：http://hz.jlsjyb.cn/gtqywmuorb.html

esac
来源：http://hz.haohaochexian.top/gtttxcsqaq.html

[R12] for 遍历文件
来源：http://hz.smart0.xyz/gtfaqclaqf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cashguo.top/gthsuackdh.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtldgwltxi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtjafrilex.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtamdmtlyt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtropilghs.html

[R15] while 逐行读文件
来源：http://hz.shzxlz.cn/gtkveqvpwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ivvv.top/gtjitascpg.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtwdcnhioz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtrbwxgxgb.html

[R17] 数组定义与取值
来源：http://hz.svipenyu.cn/gthvbvaliu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cqqwz.cn/gtqmsdiuhz.html

[R18] 遍历数组
来源：http://hz.jqgfzy.top/gtfxojkmuz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigufen.top/gttldozrdg.html

[R19] 数组长度
来源：http://hz.jqgfzy.top/gtrcexegkw.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtkabyzasi.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gtfdoonymo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gtrqdxnogs.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gtyudoreom.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtxdttgrwv.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtwmuexllj.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gtnonjmmva.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gtcyrbergd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gtehywutwd.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtueqzycwb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtswquvxdm.html

[R25] 去后缀 / 去前缀
来源：http://hz.smart0.xyz/gtvgxyrnlz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtblcnwxdj.html

[R26] 命令替换
来源：http://hz.jinqigufen.top/gtjmfcuyvx.html

now=$(date +%F); echo "$now"
来源：http://hz.gotoacloud.top/gtaoxezxnq.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gtxfcxzwth.html

echo $((1 + 2 * 3))
来源：http://hz.jyoumei.cn/gtbfqfwbug.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtekhsrrzg.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtioatjnsr.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtirbmlcoi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tanke756.top/gtmnfmzvkz.html

[R30] 函数返回状态码
来源：http://hz.jqgufenzy.top/gthyagbkft.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuxming.cn/gthpjivmyo.html

[R31] 局部变量
来源：http://hz.zhijiandao.cn/gtwssimyzt.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnxiangtu.top/gtkcaicsts.html

[R32] 参数个数校验
来源：http://hz.xingfuxueyuan.xyz/gtuarodvjo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenlongwang.top/gtrsamlacp.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gtajkpubnv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.birdmap.top/gtgzizpaus.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtverrxkjz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtycswbumk.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gttsbrduaa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtyjzwmmia.html

[R36] 并发执行多个任务
来源：http://hz.xingfuxueyuan.xyz/gtevcjvpxy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dianchejie.cn/gtnvfozryf.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtluzrspzb.html

files=$(ls -1)
来源：http://hz.shanyushiyangtech.top/gtehmcvlfs.html

[R38] 管道串联
来源：http://hz.ivvv.top/gtuxxcabsj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aibaodan.cn/gtshpkpczi.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtxmncjdir.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gtxtsooqhz.html

[R40] 追加写日志
来源：http://hz.zdqjudy.top/gttcxivggx.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gtyzoesnch.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangtech.top/gtokjntafd.html

cmd >/dev/null 2>&1
来源：http://hz.xylfe.cn/gtcutquxku.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtcqpyflxy.html

wc -l < a.txt
来源：http://hz.pycfn.com/gtsiesfluw.html

[R43] 按名字查找文件
来源：http://hz.zhiwuduotai.top/gtphvoqdqe.html

find . -name "*.log" -type f
来源：http://hz.gaohongyu789.top/gttmsbaptb.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gtmlcpzzkb.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gtnouvotaw.html

[R45] 批量删除
来源：http://hz.yj20258.top/gtuigqsbtz.html

find . -name "*.tmp" -delete
来源：http://hz.sxryk.cn/gtvfzhtwsr.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtilytgkrz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtuhrhniny.html

[R47] sed 单行替换
来源：http://hz.zhijiandao.cn/gtxunlfzhp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aizwys.cn/gttodpwzor.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtqyhfcgeh.html

awk '{print $1, $3}' a.txt
来源：http://hz.svipenyu.cn/gtqohossdw.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtumgfqayz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenjidiqi.icu/gttlsipljz.html

[R50] awk 求和
来源：http://hz.sweek.top/gtajajahoh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtpjcujxzs.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gttqnqkdbz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtapnwxviu.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtzxhbttpt.html

wc -l a.txt
来源：http://hz.mhx1999.top/gtmvwxdwcp.html

[R53] 查看文件头与实时尾
来源：http://hz.52xcode.cn/gtyhkytaze.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtqxaoyajq.html

[R54] 比较两个文件
来源：http://hz.jiagoushi.top/gttorvvbuu.html

diff a.txt b.txt
来源：http://hz.ydjk.org.cn/gtsfwzzpaq.html

[R55] 压缩与解压
来源：http://hz.yanxiufei.cn/gtzpvcnnav.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtdouniopj.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtppzyyvfr.html

scp file user@host:/path/
来源：http://hz.jinqigufen.top/gtwdfqwkwo.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtjlbezula.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gtmwawykun.html

[R58] 下载文件
来源：http://hz.zhaomingkeji.xyz/gtcvshqexp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gtfbzorbvu.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtvuahwqsp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenjidiqi.icu/gtxpodnvvz.html

[R60] 只看 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtuumthqax.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtafmnxoib.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtbfqnovbs.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtmyuwrdcp.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gthinqwtiw.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtdezrjcry.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtyeezdboq.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtpziqwbwv.html

[R64] 结束进程
来源：http://hz.tanke756.top/gtbxsfjumj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtidsbhhgt.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gthdirznpb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gogol.net.cn/gtlrbngrup.html

[R66] 定时任务
来源：http://hz.cheryme.top/gtooizopdn.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtxipvjxkv.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtmixmntko.html

openssl rand -hex 16
来源：http://hz.9152youxi.cn/gtpehibfaf.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gtyzlayvtd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhiwuduotai.top/gtlmzikdwh.html

[R69] 生成随机密码
来源：http://hz.hywenlv.cn/gtxapphdsp.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtzaalicry.html

[R70] 时间戳与互转
来源：http://hz.yuanzhike.top/gtgfeyomvg.html

date +%s;  date -d @1700000000
来源：http://hz.sweek.top/gtirkehiwg.html

[R71] 日期格式化
来源：http://hz.gzhubu.top/gtpxybkzsl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gtuebbkicf.html

[R72] 等待端口就绪
来源：http://hz.xingfuxueyuan.xyz/gtdgmdpotr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtnejnulxr.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtdqmbejys.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtiumfhewn.html

[R74] 批量重命名
来源：http://hz.tanke756.top/gtgwwuogti.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtwmfbxmrh.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtfxgxbxfg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.svipenyu.cn/gtyvqhwmph.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtejgyghph.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtvhzqcgfq.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtrbetotzc.html

read -rp "请输入: " ans
来源：http://hz.gogol.net.cn/gtxqlaigmt.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtcmnyppcm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtcelprhgr.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gtzrtrhcnj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gtuflobvyj.html

[R80] 查看脚本执行耗时
来源：http://hz.quarkkingdee.top/gtygotqloy.html

time ./run.sh
来源：http://hz.ivvv.top/gtaeagqgln.html

================================================================================
来源：http://hz.52xcode.cn/gtovqpjvmu.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtgudbffka.html

================================================================================
来源：http://hz.cdnleiting.top/gtqamvdrhp.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtralqbepu.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtokqsoaxn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtjtbatykq.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtiisxfaeo.html

int a = 10; printf("%d\n", a);
来源：http://hz.xylfe.cn/gtnkceehqw.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtjbqzjtxf.html

int x; scanf("%d", &x);
来源：http://hz.jinqigfzy.top/gtjbsijhzb.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtozvqzrdm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shuidangran.top/gtbzpmbbeu.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtygzofqmi.html

strlen(s)
来源：http://hz.ppjwa.cn/gtffxaosih.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtoegbaxjw.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtbvcufegf.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gtvwpiiifv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtglrpzmki.html

[S08] C：动态内存分配与释放
来源：http://hz.zhixingplan.top/gtacbutmrh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtvbpuvyeu.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtrjefwxxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtyfxnajeq.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtxcdhjniz.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtgtpyaxwy.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtvzjaiegb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuanzx.com/gtpmrrppth.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtkkeebaks.html

fclose(f);
来源：http://hz.jqgfzy.top/gtggctevld.html

[S12] C：写文件
来源：http://hz.yvedp.cn/gtfnsjeked.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtjgrnppgy.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtzkdajvul.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daria6918.cn/gtvzzqkdva.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtlklbfpzq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.c1oappe.top/gtkucgrmrr.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtognafpka.html

(double) a / b
来源：http://hz.hfpthk.cn/gtrjjhsjyn.html

[S16] C：位操作置位
来源：http://hz.hongshengwenyu.top/gtwonjiuhm.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gtghqxrtqu.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gtzqbgtyys.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fengsongda.top/gtfebtkeob.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtsyjaakpt.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtlqfyhmyn.html

[S19] C：快速排序
来源：http://hz.meibo888.top/gtzxwvhcux.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtnlcuaslf.html

[S20] C：二分查找
来源：http://hz.smart0.xyz/gthsmwljou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gttwlzazpc.html

[S21] C：字符类别判断
来源：http://hz.feifeiyinyue.top/gtmxkuwzwg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yongpay.top/gtgfrfifie.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtuimnjbin.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gttqrgbphr.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gtczytnfso.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gttsvjhjeu.html

[S24] C：获取本地时间
来源：http://hz.zhongyouzk.top/gtlcqianul.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhoulong.xyz/gtheqtgfwd.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtjatmpqjl.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtjxozeebf.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtxtryaokx.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtgeiujekc.html

[S27] C：定义常量
来源：http://hz.sweek.top/gtcroubahb.html

const double PI = 3.14159;
来源：http://hz.ehwqpu.com/gtgipakhli.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtkcdknfle.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtvrkudsou.html

[S29] C：变参函数
来源：http://hz.kuanghao11.cn/gtpuorxbuz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.9152youxi.cn/gtmcjrdpyr.html

[S30] C：头文件保护
来源：http://hz.9152youxi.cn/gttduttvnk.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtdadfocqj.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtexnazsok.html

#endif
来源：http://hz.andypj.xyz/gtunzdieqf.html

[S31] C++：Hello World
来源：http://hz.yj202588.top/gthcdxjnkt.html

#include <iostream>
来源：http://hz.smart0.xyz/gtoyluxyie.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtoxylzfnr.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtitfntluo.html

std::string s = "hi";  s += "!";
来源：http://hz.ywan-chungtsiang.top/gtodzqkowq.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gtbqukxity.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.52xcode.cn/gttrcmepik.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtaxkwvhkn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtyegmddlh.html

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtwtrekwto.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtlazxuxoz.html

[S36] C++：unordered_map
来源：http://hz.xziqi.cn/gtnoelnisn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtgnhhuvox.html

[S37] C++：set
来源：http://hz.vqdsnc.cn/gtsrvgioim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtrqceoxxg.html

[S38] C++：排序
来源：http://hz.haohaochexian.top/gtosijenmz.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtzsxpaqxh.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgfzy.top/gtleiprlsg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cheryme.top/gttkebhhys.html

[S40] C++：查找元素
来源：http://hz.iojbl.cn/gtbofcjkkv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtsqcmxzhw.html

[S41] C++：类与构造函数
来源：http://hz.jqgufenzy.top/gtbtagvlbv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtckfclbtb.html

[S42] C++：继承与虚函数
来源：http://hz.yvedp.cn/gttaovarnh.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtpqqyxlxm.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtfqrelmod.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtixrvlzvc.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtajpgpebo.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtulbwvnyx.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtriiisucq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zdqjudy.top/gttofyctrs.html

[S46] C++：函数模板
来源：http://hz.yj20258888.top/gttvkjuibl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtuklnvehb.html

[S47] C++：结构化绑定遍历
来源：http://hz.tanke756.top/gtakvynakz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtzauppkvq.html

[S48] C++：逐行读文件
来源：http://hz.xziqi.cn/gtlvylswiu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guannengcc.top/gtvsjpiiet.html

while (std::getline(in, line)) { }
来源：http://hz.chenjidiqi.icu/gtuninpuly.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtedcztcuw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtzcdyjhsv.html

[S50] C++：格式化数字
来源：http://hz.birdmap.top/gtytnuyuoh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtdcxvedzs.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gteqzcvkmy.html

static_cast<double>(a) / b
来源：http://hz.zycfv.cn/gtckhcqpju.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtmbdbqkvt.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gtfbxplcdn.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtoyamgpcd.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258888.top/gtxtkzlyag.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtpmvaimqx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtxfekuykc.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtncclftgy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangdashe.top/gttxyuywmg.html

[S56] C++：optional
来源：http://hz.fengsongda.top/gtbedvvecr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gttxycxari.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtloasxpfr.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtxoessoms.html

[S58] C++：命名空间
来源：http://hz.cheryme.top/gtscmibsoq.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtejaprgnp.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtxdhajaux.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtdjbqkwym.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtwjkyxylr.html


<!-- 参考信息 -->