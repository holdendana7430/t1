代发 wailian999

R. Bash 专题
来源：http://hz.ydzc1.top/gtcnmyhwoh.html

================================================================================
来源：http://hz.xziqi.cn/gthatvmwih.html

[R01] shebang 与严格模式
来源：http://hz.mhx1999.top/gthdfvgndz.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtqutpjjpe.html

set -euo pipefail
来源：http://hz.xziqi.cn/gttfsnpmdk.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtdaxlwdkf.html

name="Tom"; echo "$name"
来源：http://hz.hongshengwenyu.top/gtrrfbklxy.html

[R03] 只读变量
来源：http://hz.gaohongyu789.top/gtswvklgds.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gtyoiqmabh.html

[R04] 位置参数
来源：http://hz.yongpay.top/gtmclorsti.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxuanxn.top/gtpfyjmwpi.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtxdwiwyrg.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtozuaghem.html

[R06] 判断命令是否存在
来源：http://hz.hongshengwenyu.top/gtzsozngct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.smart0.xyz/gtvijmzdfz.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtzdavnydo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.nanxinkj.top/gtbnmosopz.html

[R08] 数值比较
来源：http://hz.yonumen.top/gtlsaodbmd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jlsjyb.cn/gtgvjtbylj.html

[R09] 字符串比较
来源：http://hz.yanxiufei.cn/gtocqyrqgo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtaowfobxm.html

[R10] 正则匹配
来源：http://hz.birdmap.top/gtwxaekbti.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtwwmionxr.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtgozsqoau.html

case "$1" in
来源：http://hz.shangyingyoupin.top/gtllpxmxzd.html

start) echo "启动" ;;
来源：http://hz.cashguo.top/gtolpyvaio.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtdezjibyb.html

*)     echo "未知命令" ;;
来源：http://hz.zhoulong.xyz/gtykvmqwyj.html

esac
来源：http://hz.cucudq.cn/gtwohpnmjn.html

[R12] for 遍历文件
来源：http://hz.jqgfzy.top/gtwkeuvrim.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jqgfzy.top/gthbigwkkk.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtrcbkvejv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.svipenyu.cn/gtqdecvnyt.html

[R14] C 风格 for
来源：http://hz.xziqi.cn/gtivgoqsyj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtpddahvcv.html

[R15] while 逐行读文件
来源：http://hz.jinqigfzy.top/gtnmkwdfft.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtefclbkog.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtqqtdbkin.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.haohaochexian.top/gtiecrwsbk.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtcrmunbxw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtubdxgpyx.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtdnzbdwru.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gttydelfuw.html

[R19] 数组长度
来源：http://hz.zycfv.cn/gtitdygbmx.html

echo "${#arr[@]}"
来源：http://hz.aizwys.cn/gtqjwvigra.html

[R20] 关联数组（字典）
来源：http://hz.mhx1999.top/gtccqgvvud.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fengsongda.top/gtngaeyqgx.html

[R21] 字符串长度
来源：http://hz.sufxvd.cn/gtelbdrvww.html

echo "${#s}"
来源：http://hz.ydzc1.top/gtwkyrrwcg.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gtpdbkfwre.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtbhigichc.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtrnohzlke.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigfzy.top/gtwganwvje.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtataozzqr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtcfyvkulc.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtkxbsowcn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gtzskmknlk.html

[R26] 命令替换
来源：http://hz.havefunace.top/gtylcskkdj.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtjhpbxzry.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtmbppdxes.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtmbyeyppo.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtvgpsnigu.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtnqdrocyn.html

[R29] 定义函数
来源：http://hz.aibaodan.cn/gttjultgbt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sweek.top/gtpzvoafvp.html

[R30] 函数返回状态码
来源：http://hz.gogol.net.cn/gtlaxrlwht.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtneysshud.html

[R31] 局部变量
来源：http://hz.havefunace.top/gtvmhatqsx.html

f() { local x=1; echo "$x"; }
来源：http://hz.pengpengdd.cyou/gtonibxaxf.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtbprdhmxs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtndbrmumi.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtarizrxld.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtznzernbk.html

[R34] 退出时清理
来源：http://hz.xuanzx.com/gtqhowyoih.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtvqedlgsu.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtclesngjd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cqqwz.cn/gtjeyqremn.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtfshyylwa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zdqjudy.top/gtgzandpgc.html

[R37] 把输出赋给变量
来源：http://hz.jqgufenzy.top/gtnkmvoiet.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtcewjydsq.html

[R38] 管道串联
来源：http://hz.zhongyouzk.top/gtmiftoivl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gtozcvwsod.html

[R39] 重定向标准输出与错误
来源：http://hz.dashuyun.cn/gtvbkaaady.html

cmd > out.log 2>&1
来源：http://hz.snrcjt.cn/gtcbqnwnsj.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtasixxxkd.html

echo "log" >> out.log
来源：http://hz.daria6918.cn/gtsomjddws.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtwwqybfha.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtdqkihfyr.html

[R42] 输入重定向
来源：http://hz.sweek.top/gtdklwsghm.html

wc -l < a.txt
来源：http://hz.yj20258888.top/gtxxwokexq.html

[R43] 按名字查找文件
来源：http://hz.cdnleiting.top/gtdgqgitld.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtalcskadg.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtavkehmvh.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtgcjsmglz.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtuvumraef.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtvqmsdfgq.html

[R46] 递归替换文件内容
来源：http://hz.hysaishi.cn/gtzadrptgg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtfnpqheiv.html

[R47] sed 单行替换
来源：http://hz.chenzaomai.com/gthdglbeoa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtfsgxgevp.html

[R48] awk 取指定列
来源：http://hz.shzxlz.cn/gtfisyyszh.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtftwvtiyf.html

[R49] awk 带条件
来源：http://hz.bjfxy.top/gtrkajuodx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ybcxt.top/gtnfbcbllq.html

[R50] awk 求和
来源：http://hz.xylfe.cn/gtdlugvlnn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuetiantiany.cn/gtnutjsbor.html

[R51] 排序去重取前几
来源：http://hz.xziqi.cn/gtdnsmlcaa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gtbeumijzi.html

[R52] 统计行数
来源：http://hz.yangfankeji.com/gtqxmzjqym.html

wc -l a.txt
来源：http://hz.zhixingplan.top/gtllqqaclr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtuetawain.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtwgyvavte.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtehnhovgy.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtykfxfwvo.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtaulbgmjk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.haohaochexian.top/gtgnytqfwz.html

[R56] 远程拷贝
来源：http://hz.hysaishi.cn/gtwptjsitu.html

scp file user@host:/path/
来源：http://hz.52xcode.cn/gtirjybhpt.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtpvxeacik.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtmmthjtyq.html

[R58] 下载文件
来源：http://hz.redwolf501.top/gtyuhtaewl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtluheqoeu.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtqpgudubs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtbmolatru.html

[R60] 只看 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtjyytsohq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtircupvck.html

[R61] 磁盘占用
来源：http://hz.zhengqikj.top/gtmtwoaola.html

df -h;  du -sh *
来源：http://hz.jianghu66.top/gtnpcstzks.html

[R62] 找最占空间的文件
来源：http://hz.fengsongda.top/gtwjuvemws.html

du -ah . | sort -rh | head -10
来源：http://hz.meibo888.top/gtjdvvsmcf.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtqawtzaei.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtutyfowob.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtgrruznxs.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fzhhl.top/gtcmkzxvij.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtmtimsxtw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtzliizqdm.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtfbouiczc.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtabfuywhb.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gtjpjiaokw.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtbacpxxsv.html

[R68] 计算文件校验值
来源：http://hz.jlsjyb.cn/gthbbzrrlm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtczmlqwob.html

[R69] 生成随机密码
来源：http://hz.0kj1m.cn/gtftvlcvty.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtpzievrom.html

[R70] 时间戳与互转
来源：http://hz.zhengqikj.top/gtbnsgwkxe.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtzecogfhi.html

[R71] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtgtxxejyy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pengpengdd.cyou/gtqsnjpdvh.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtmhshoqqu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gturigseoc.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtkvuekplg.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtrcfchila.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gthgkyqatj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gttzygzupg.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtjhjlduyc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtooceodhu.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtdwjibcma.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtlouydwbp.html

[R77] 读取用户输入
来源：http://hz.hywenlv.cn/gtsgwatmiw.html

read -rp "请输入: " ans
来源：http://hz.aibaodan.cn/gtcyayucjw.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtgwdrisbb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenjidiqi.icu/gthqxnjsuc.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtkqlqgeps.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hysaishi.cn/gtedyvloob.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtubqkfmfu.html

time ./run.sh
来源：http://hz.jinqigufen.top/gtxmyswmnv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfitbnltc.html

S. C / C++ 专题
来源：http://hz.zhaomingkeji.xyz/gtpzkenujg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbtnudefi.html

[S01] C：Hello World
来源：http://hz.pycfn.com/gthsphjmmc.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtvqhfuqhx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxuanxn.top/gtybvlhuzg.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtvcpuylyj.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtlprrfxff.html

[S03] C：读入整数
来源：http://hz.pengpengdd.cyou/gtqdxpnutb.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtdyhugppy.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtjiznqdwa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtlwyjagqj.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtvkuivzbc.html

strlen(s)
来源：http://hz.c1oappe.top/gtkruynzaf.html

[S06] C：字符串比较
来源：http://hz.hfpthk.cn/gtqtupwmqx.html

strcmp(a, b) == 0
来源：http://hz.ydjk.org.cn/gtdurotzpo.html

[S07] C：数组遍历求和
来源：http://hz.316326.xyz/gthfbtwxtj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gtaztnrtms.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangtech.top/gtvwltscxr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenzaomai.com/gtpgosyrmt.html

[S09] C：结构体定义与初始化
来源：http://hz.cashguo.top/gtxaajskbx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtudgbxqrh.html

[S10] C：指针与解引用
来源：http://hz.ybcxt.top/gtfpdnecer.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtzdrywgmr.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtczxrplbd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gtnjyntlqc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jyoumei.cn/gtwoceuuxz.html

fclose(f);
来源：http://hz.jianghu66.top/gtkjwmkrlv.html

[S12] C：写文件
来源：http://hz.mhx1999.top/gttvedlbwh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtyrokujjm.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gtffgdqzzl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigfzy.top/gtzifpazts.html

[S14] C：枚举
来源：http://hz.andypj.xyz/gtgirhwltp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.0kj1m.cn/gtmtsnopnb.html

[S15] C：类型转换
来源：http://hz.ywan-chungtsiang.top/gtahjgvqvb.html

(double) a / b
来源：http://hz.cucudq.cn/gtlezrlvmr.html

[S16] C：位操作置位
来源：http://hz.ivvv.top/gtfbbdajrh.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtkopqskap.html

[S17] C：安全拼接字符串
来源：http://hz.ydjk.org.cn/gtljjhlrdc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtobmwbmay.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtjfxjayxa.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtfzmkmros.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gtjhjlugyk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtfihrgcrs.html

[S20] C：二分查找
来源：http://hz.aizwys.cn/gtqhjcsfmc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtdwvmmvzt.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtkdilwgsa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.havefunace.top/gtnleycnlp.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtlfhzechi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtsdxqssta.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtkqflicdh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtevsqgpak.html

[S24] C：获取本地时间
来源：http://hz.svipenyu.cn/gtuwsosljw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nwbrower.top/gteolhvgob.html

[S25] C：内存拷贝
来源：http://hz.iojbl.cn/gtfgucuxfk.html

memcpy(dst, src, n);
来源：http://hz.yvedp.cn/gtsocplcmv.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtvrdfxnhv.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtdyfbrltu.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtcxavfxkg.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtiyfvmkft.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtyuoukmdz.html

static int counter = 0;
来源：http://hz.smart0.xyz/gttgntarlm.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtcyfuwbnd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtodstuujg.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gttbxuzeao.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gtzwldamtv.html

#define X_H
来源：http://hz.shuidangran.top/gtmgkeweeb.html

#endif
来源：http://hz.nwbrower.top/gtiyqpjsyx.html

[S31] C++：Hello World
来源：http://hz.pycfn.com/gtshpmwvyv.html

#include <iostream>
来源：http://hz.jianghu66.top/gtunosuzdq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sysykeji.top/gtbakauyic.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtgbpscmjw.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtroqkcnpj.html

[S33] C++：vector 增删
来源：http://hz.pengpengdd.cyou/gtupxbgnzc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtvdtcxbnt.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtgyvhvfag.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtwwobevvz.html

[S35] C++：map
来源：http://hz.shanyushiyangtech.top/gtrwrsqoml.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gttunkupur.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtvjzcgzux.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtwguaiant.html

[S37] C++：set
来源：http://hz.mhx1999.top/gttmabarzf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtpwprtdzf.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gttpwpxmlq.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gtmerubnjw.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtrovyjdmm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xziqi.cn/gtyuibesnf.html

[S40] C++：查找元素
来源：http://hz.smart0.xyz/gttwmptuzj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhoulong.xyz/gtavbbqmuo.html

[S41] C++：类与构造函数
来源：http://hz.yj20258888.top/gtwavwfahe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jianghu66.top/gtndxyvcmb.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtzzbskjgj.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtypuwdszd.html

[S43] C++：智能指针
来源：http://hz.zhongyouzk.top/gtswrvuaqp.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtrkfzqagu.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtxbqfwxct.html

void inc(int &x) { ++x; }
来源：http://hz.ppjwa.cn/gtgrytkgdu.html

[S45] C++：lambda
来源：http://hz.xinyue.icu/gtsoothtjk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtydirfpnc.html

[S46] C++：函数模板
来源：http://hz.tianlin.xyz/gthnpaqexz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenjidiqi.icu/gtjlhlwdoq.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtibaukrye.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yvedp.cn/gtmlxocywp.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gtgsceigyz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtufbkynsa.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtwncjqqpc.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtpcwheqtx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtjboarkuv.html

[S50] C++：格式化数字
来源：http://hz.gaohongyu789.top/gtbpftpylg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtzlljqjbq.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtesvciqdd.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtgdwancrf.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtiklqtdew.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtxvrjrbpw.html

[S53] C++：移动语义
来源：http://hz.zycfv.cn/gtdhjeihey.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtcasljnyd.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtqnqcdqbe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtvfwfjsof.html

[S55] C++：结构化绑定
来源：http://hz.xziqi.cn/gtzrsuxpro.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nwbrower.top/gtvbkcngle.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtqmtjzwdg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258888.top/gtibkmvqdb.html

[S57] C++：编译期常量
来源：http://hz.cqqwz.cn/gtqgpxxguq.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gteauqaabe.html

[S58] C++：命名空间
来源：http://hz.guowangkeji.top/gtqpzzlagk.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinghuilouyu.cn/gtgsgrydef.html

[S59] C++：静态断言
来源：http://hz.hongshengwenyu.top/gtvhuribdn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yvedp.cn/gtlzlaqrii.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtykxnvbal.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtajkdkudq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtquqwfeci.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtfqgpnyxy.html

================================================================================
来源：http://hz.316326.xyz/gtaeplpkef.html


<!-- 参考信息 -->