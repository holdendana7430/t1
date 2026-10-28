代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.quarkkingdee.top/gtpqoxlook.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gtfqyqwppb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hongshengwenyu.top/gtxitsazcv.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtsgsjxnrr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tanke756.top/gthlhemfuj.html

[Q90] 生成序号列
来源：http://hz.yongpay.top/gthowyopns.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gotoacloud.top/gtiwbdlbtk.html

================================================================================
来源：http://hz.xuanzx.com/gtwlrwtyrx.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtdmpfmgfq.html

================================================================================
来源：http://hz.ehwqpu.com/gtkfkrxclb.html

[R01] shebang 与严格模式
来源：http://hz.snrcjt.cn/gtxyjxakor.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtryixbrsr.html

set -euo pipefail
来源：http://hz.hysaishi.cn/gtypdxkfwb.html

[R02] 变量赋值与使用
来源：http://hz.hammf.cn/gtyysekyva.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtqeaouvzm.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtfeaenreo.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtlfxcejxo.html

[R04] 位置参数
来源：http://hz.ywan-chungtsiang.top/gtkartbevd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtoiqwsxrh.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gturhlgfhz.html

name="${1:-default}"
来源：http://hz.zhongyouzk.top/gtiupmemkq.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gtvauchbac.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtarsylqjh.html

[R07] if 判断文件
来源：http://hz.feifeiyinyue.top/gtqexeqjtb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.kuanghao11.cn/gtodgmypvg.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtezqvpmgw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtkwbzcuml.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtylftudyt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zycfv.cn/gtbfvkgadw.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtcmkvxuhe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gtkazqtlpx.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtpsghsfue.html

case "$1" in
来源：http://hz.gotoacloud.top/gtlonjhwdc.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtokgbgcyn.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtosziqvwe.html

*)     echo "未知命令" ;;
来源：http://hz.ydzc1.top/gtaeihpjbx.html

esac
来源：http://hz.pycfn.com/gtvqcyecaq.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gthffhyfxc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtpsxjnaxa.html

[R13] for 计数循环
来源：http://hz.hammf.cn/gtywitepcq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtfzqcvdpt.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gttgddciok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.tianlin.xyz/gtnqunggit.html

[R15] while 逐行读文件
来源：http://hz.cqqwz.cn/gtazanbytv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtzrhscleu.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtoqrcyjrj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtjgryilbb.html

[R17] 数组定义与取值
来源：http://hz.feifeiyinyue.top/gtybbuasfi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gaohongyu789.top/gtamfswtvk.html

[R18] 遍历数组
来源：http://hz.jiagoushi.top/gtbziakvlb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hysaishi.cn/gtpmzyeqhg.html

[R19] 数组长度
来源：http://hz.fengsongda.top/gtoyvjhyym.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtihhoddvi.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gtbkpncpbm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuanzhike.top/gtxsiuavvd.html

[R21] 字符串长度
来源：http://hz.ivvv.top/gtdkwodznu.html

echo "${#s}"
来源：http://hz.tanke756.top/gtsugosyof.html

[R22] 截取子串
来源：http://hz.ehwqpu.com/gtsedtyvhj.html

echo "${s:0:5}"
来源：http://hz.hysaishi.cn/gtxdwnhqbw.html

[R23] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtfedhidoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtmexwjbow.html

[R24] 大小写转换
来源：http://hz.andypj.xyz/gtzpltfrdv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydzc1.top/gtqxrftxye.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtxotchrbc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.redwolf501.top/gtbdeeirfy.html

[R26] 命令替换
来源：http://hz.hysaishi.cn/gtpzelfdev.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gtzvglkzpd.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtxxlmmwuf.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gtwuggsago.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtmrgedurx.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinghuilouyu.cn/gtzolswltr.html

[R29] 定义函数
来源：http://hz.yj202588.top/gtlgfuwdja.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangkeji.top/gtxdkztryu.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtatlinzjd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yvedp.cn/gtetncftrk.html

[R31] 局部变量
来源：http://hz.hnxiangtu.top/gtlnqhyvyz.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtxleajtci.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtarwtdczl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtlqkcombv.html

[R33] 捕获错误并提示行号
来源：http://hz.xuanzx.com/gtqwaesqzd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtdmxryjwj.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtppjtcpgm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtsmelygab.html

[R35] 后台执行并等待
来源：http://hz.pycfn.com/gtnkrqbuqj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258.top/gtzkabuoov.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtghlvrkcx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj202588.top/gtcqbfqxtf.html

[R37] 把输出赋给变量
来源：http://hz.jiagoushi.top/gteiysjgdc.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtzukponpe.html

[R38] 管道串联
来源：http://hz.jyoumei.cn/gthmflkqtl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gtyvkcoqps.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigufen.top/gttxmbjbsm.html

cmd > out.log 2>&1
来源：http://hz.ydjk.org.cn/gtxsunsaps.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtvczjuvsf.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtkxoupcae.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtrwzlysib.html

cmd >/dev/null 2>&1
来源：http://hz.vqdsnc.cn/gtxnqdgwtu.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtoqecnvlz.html

wc -l < a.txt
来源：http://hz.cheryme.top/gtzxrzfiwc.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtvmqqttdt.html

find . -name "*.log" -type f
来源：http://hz.chenlongwang.top/gtbttusypn.html

[R44] 按修改时间查找
来源：http://hz.zhiwuduotai.top/gtbfipeann.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtuntyjcmg.html

[R45] 批量删除
来源：http://hz.vqdsnc.cn/gtlfzwitjv.html

find . -name "*.tmp" -delete
来源：http://hz.cheryme.top/gtdmlsajag.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtdntmimfk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cqqwz.cn/gtjeyowica.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gthzdzwprv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gthpnvopdz.html

[R48] awk 取指定列
来源：http://hz.meibo888.top/gtljniqjhg.html

awk '{print $1, $3}' a.txt
来源：http://hz.ybcxt.top/gtnqxtirnu.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtsuqocmto.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtivpkxtwo.html

[R50] awk 求和
来源：http://hz.tianlin.xyz/gtdladhicv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gttwmwblbw.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtlhfljltt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtbssuxxjh.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtjpwyadmo.html

wc -l a.txt
来源：http://hz.feifeiyinyue.top/gtmfmgtjoj.html

[R53] 查看文件头与实时尾
来源：http://hz.gotoacloud.top/gtjnumddqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.316326.xyz/gtppsgcqyy.html

[R54] 比较两个文件
来源：http://hz.nanxuanxn.top/gttuzjccsm.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtdgdtvgrt.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangtech.top/gtdelicqgx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jiagoushi.top/gtofsxqddr.html

[R56] 远程拷贝
来源：http://hz.jinqigufen.top/gtsiktjttb.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtxiqntbsf.html

[R57] 远程执行命令
来源：http://hz.hnqzz.top/gtxuiuvzqs.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtygyokksc.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtylgbnwou.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.andypj.xyz/gtohmwkjbf.html

[R59] 发 POST JSON
来源：http://hz.jinqigfzy.top/gtdusadkdy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.mhx1999.top/gtrnrcosfz.html

[R60] 只看 HTTP 状态码
来源：http://hz.cucudq.cn/gtymcinong.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtleluovle.html

[R61] 磁盘占用
来源：http://hz.xziqi.cn/gtpgahcjcf.html

df -h;  du -sh *
来源：http://hz.aizwys.cn/gteapmjotj.html

[R62] 找最占空间的文件
来源：http://hz.c1oappe.top/gtqciyxgbm.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtnfbdfofc.html

[R63] 内存与进程
来源：http://hz.aibaodan.cn/gtxatogtwq.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtitbvgusp.html

[R64] 结束进程
来源：http://hz.yj202588.top/gtsnhsbixv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtnsradypr.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtdbnfxqeg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtbhqtxtau.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtprlnpuci.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtcifednlg.html

[R67] 生成随机十六进制串
来源：http://hz.chenlongwang.top/gtkkdabrdm.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gtwqobtmuv.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtfbsxitvs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtsvqvlvur.html

[R69] 生成随机密码
来源：http://hz.zhoulong.xyz/gtstpljufr.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtrtmlqpid.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtwdspycfp.html

date +%s;  date -d @1700000000
来源：http://hz.52xcode.cn/gtfrascsam.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtnhmcbadi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtzfcgrirq.html

[R72] 等待端口就绪
来源：http://hz.kuanghao11.cn/gtlrgnpcvs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtvkmnvmrx.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtomplenfn.html

split -l 1000 big.log part_
来源：http://hz.jyoumei.cn/gtiuwzsjlq.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtmfiishfa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtrzkeurvh.html

[R75] 导出环境变量
来源：http://hz.shzxlz.cn/gtcmygibkg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xylfe.cn/gtryiwjyvk.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtsadktync.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtkbbccdca.html

[R77] 读取用户输入
来源：http://hz.jinghuilouyu.cn/gtuogcebtl.html

read -rp "请输入: " ans
来源：http://hz.sufxvd.cn/gteobrsiyj.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gtrcdvmhrq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gtzzhqjlhs.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtpdhxdnom.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gtnsvpcvsj.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtxhoeumgl.html

time ./run.sh
来源：http://hz.tianlin.xyz/gtdnnwnqtm.html

================================================================================
来源：http://hz.yuxming.cn/gtcvbhwrlw.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtkfysuumy.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtomhsxccc.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtdbkstula.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtaqkyymah.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtausktnti.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtezatkwqn.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtgzsczilw.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gtobsglgaf.html

int x; scanf("%d", &x);
来源：http://hz.dianchejie.cn/gtjthzkrhk.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtncncyzfw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guannengcc.top/gttaiywhxl.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtjjdfhgtp.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtjgiqkmsw.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtsjujyjjs.html

strcmp(a, b) == 0
来源：http://hz.c1oappe.top/gtkqyneakp.html

[S07] C：数组遍历求和
来源：http://hz.gaohongyu789.top/gtxxxnyqxg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtzxydgnkg.html

[S08] C：动态内存分配与释放
来源：http://hz.haohaochexian.top/gtinbydujt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtzdwrqbns.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtzwizhpmf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtzwqstaoj.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gtpnpgbyan.html

int *p = &a;  *p = 5;
来源：http://hz.cucudq.cn/gtdihlyeci.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtvlqbrbmk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtzxvelndr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtvggizjwq.html

fclose(f);
来源：http://hz.shuidangran.top/gtphmulxqy.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtjojduxrw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtumcocuxx.html

[S13] C：宏定义
来源：http://hz.xziqi.cn/gtixxclsqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hfpthk.cn/gtvtynibsl.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtonhfjdyb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gtwrfgteti.html

[S15] C：类型转换
来源：http://hz.svipenyu.cn/gtvvgdufdl.html

(double) a / b
来源：http://hz.haohaochexian.top/gtytdxgowt.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gtrgyelopw.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtlhdrtmur.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gtfybqgysd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cucudq.cn/gthggwuega.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtmozlglqv.html

int main(int argc, char **argv)
来源：http://hz.wangshuangyany.cn/gtsleqcutn.html

[S19] C：快速排序
来源：http://hz.cashguo.top/gtmunhzppz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gttpmoqflt.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtceymwuxf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtghextgkn.html

[S21] C：字符类别判断
来源：http://hz.jyoumei.cn/gtshrhjcfv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daxiang520.top/gtqukxdbxe.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtagijqjgz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtodeljhmo.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtckbmxzau.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtdoctczhd.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtwqkxotjm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtcablsagz.html

[S25] C：内存拷贝
来源：http://hz.hammf.cn/gtukqenpny.html

memcpy(dst, src, n);
来源：http://hz.andypj.xyz/gtjzlbzhfd.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gteyvembve.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtjehikxdq.html

[S27] C：定义常量
来源：http://hz.dianchejie.cn/gtqvmyjzog.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtqhqwnqxr.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtgsciaagk.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtppjtczit.html

[S29] C：变参函数
来源：http://hz.zycfv.cn/gtwefybjyj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nwbrower.top/gtbbckrslx.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gthsenbsfh.html

#ifndef X_H
来源：http://hz.shzxlz.cn/gtdbywxspe.html

#define X_H
来源：http://hz.daxiang520.top/gtczqkigdg.html

#endif
来源：http://hz.gzhubu.top/gtiuzdqkmo.html

[S31] C++：Hello World
来源：http://hz.shuidangran.top/gtfnwxxthq.html

#include <iostream>
来源：http://hz.c1oappe.top/gttvjfqhzf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yueranfly.top/gtlhsaqbao.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtkthzavtf.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtrdlfczka.html

[S33] C++：vector 增删
来源：http://hz.vqdsnc.cn/gtohiapjho.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pycfn.com/gtlcqfaqbk.html

[S34] C++：遍历 vector
来源：http://hz.fzhhl.top/gttbendbqd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxuanxn.top/gtwwnybumk.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtighkyvbh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtxgxrrxdy.html

[S36] C++：unordered_map
来源：http://hz.ehwqpu.com/gtghbtjoro.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtotutjrqy.html

[S37] C++：set
来源：http://hz.bjfxy.top/gtgxoooylw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtdefmblio.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gteezwjedu.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gthifufuho.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtfvmzhipv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gthhroiuod.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtalqmhkyf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cucudq.cn/gtsynimyhd.html

[S41] C++：类与构造函数
来源：http://hz.jqgufenzy.top/gtmaapgcvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yueranfly.top/gttezrwpyl.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gtbrsrrsil.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtzpntowsp.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtjmyzmfdp.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtztezhebl.html

[S44] C++：引用传参
来源：http://hz.haohaochexian.top/gtjvnkmfrg.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtqqsggwwb.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gthtcakvor.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnxiangtu.top/gttklvbzib.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtukdpsaop.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gtaicfuxtf.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gthuktvpki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zdqjudy.top/gticrfqfdf.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtptfutamh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinyuanbaomall.cn/gtecjfzazq.html

while (std::getline(in, line)) { }
来源：http://hz.cucudq.cn/gtlyzabiro.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtytqkacoz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtknjoqpmm.html

[S50] C++：格式化数字
来源：http://hz.nanxinkj.top/gtnqtziazu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhiwuduotai.top/gttcpnbfhr.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtrqtzpijo.html

static_cast<double>(a) / b
来源：http://hz.dianchejie.cn/gtylrepbkx.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtyosulcrp.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtmcocures.html

[S53] C++：移动语义
来源：http://hz.wangdashe.top/gtfddoesgv.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtgvptbbbu.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtwzhopces.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtvezsqntg.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtcfaxeusu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sweek.top/gtoccbdrbc.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gtmpugpmzq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.svipenyu.cn/gtcaijgkcm.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gtiqywugex.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtnjbfqmbh.html

[S58] C++：命名空间
来源：http://hz.xziqi.cn/gtvuinglgw.html


<!-- 参考信息 -->