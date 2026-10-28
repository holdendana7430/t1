代发 wailian999

esac
来源：http://hz.sufxvd.cn/gtgsqgldng.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtjcczjuby.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtbtsqbpth.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gtzodwdhsc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dianchejie.cn/gtyjmylmqe.html

[R14] C 风格 for
来源：http://hz.zdqjudy.top/gtgyqzxugf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hfpthk.cn/gtswzmyici.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtreljcfhe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.mhx1999.top/gtzaktqozb.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtstvwkklb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yuanzhike.top/gtcchxtjrs.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtudcbcxaf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dianchejie.cn/gtpkzxidhp.html

[R18] 遍历数组
来源：http://hz.yuanzhike.top/gtvbxbuaia.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtqzfcsajr.html

[R19] 数组长度
来源：http://hz.sysykeji.top/gtujolppze.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtucnjtzpj.html

[R20] 关联数组（字典）
来源：http://hz.chenlongwang.top/gtqxsghjiy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ppjwa.cn/gtnnpsrsre.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtufmmdguv.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtfbntgafa.html

[R22] 截取子串
来源：http://hz.meibo888.top/gtqjjmcxbf.html

echo "${s:0:5}"
来源：http://hz.jiagoushi.top/gteszxmcxc.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gtcxgksiaf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtucxvuzkn.html

[R24] 大小写转换
来源：http://hz.jiagoushi.top/gtsdiajmbo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.bjfxy.top/gtwivuxegx.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhengqikj.top/gtrtlgvkih.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtnicobsyl.html

[R26] 命令替换
来源：http://hz.guannengcc.top/gtzsomwcdx.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtwftmqjmp.html

[R27] 算术展开
来源：http://hz.ehwqpu.com/gtiarvilkl.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtngpbwuua.html

[R28] 浮点运算
来源：http://hz.kuanghao11.cn/gtiygpyggl.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gtcoopefda.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtngohkfwg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gtqwnixgwq.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtudhzvxur.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gtzpvydjwj.html

[R31] 局部变量
来源：http://hz.hfpthk.cn/gtkinhnpxq.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gthjasfrxa.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtvcnstabe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guowangkeji.top/gtcdwvxppy.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtsutprawl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jqgfzy.top/gtuypzpsgt.html

[R34] 退出时清理
来源：http://hz.yangfankeji.com/gtmafjxwmy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtkdsdkviz.html

[R35] 后台执行并等待
来源：http://hz.redwolf501.top/gtqeywpzbv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj20258888.top/gthnaynvrz.html

[R36] 并发执行多个任务
来源：http://hz.shangyingyoupin.top/gtpccpmxyo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtfcxlsgkl.html

[R37] 把输出赋给变量
来源：http://hz.guowangkeji.top/gtyowjyutl.html

files=$(ls -1)
来源：http://hz.hammf.cn/gtswxnekjx.html

[R38] 管道串联
来源：http://hz.gaohongyu789.top/gthphtrjni.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhiwuduotai.top/gthebkhrlq.html

[R39] 重定向标准输出与错误
来源：http://hz.yuanzhike.top/gtkxvyipmg.html

cmd > out.log 2>&1
来源：http://hz.daria6918.cn/gtpluujlat.html

[R40] 追加写日志
来源：http://hz.xylfe.cn/gtoklfjikw.html

echo "log" >> out.log
来源：http://hz.aizwys.cn/gtisxundvy.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtnhtalstn.html

cmd >/dev/null 2>&1
来源：http://hz.zhijiandao.cn/gtacxegigx.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gteaypcgwy.html

wc -l < a.txt
来源：http://hz.aizwys.cn/gteksaoesa.html

[R43] 按名字查找文件
来源：http://hz.yonumen.top/gttcacilhe.html

find . -name "*.log" -type f
来源：http://hz.ppjwa.cn/gtlupwbyva.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtsxuhchhm.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gthkrltrmd.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtkpdmtgwp.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtzdauoqsz.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtgswgpcbt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtpjbxetps.html

[R47] sed 单行替换
来源：http://hz.mhx1999.top/gtwodbxytz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinghuilouyu.cn/gtjbhnvfvv.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtcohgkqck.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtehmpexkz.html

[R49] awk 带条件
来源：http://hz.c1oappe.top/gthcohqmvd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ywan-chungtsiang.top/gtakdqqhse.html

[R50] awk 求和
来源：http://hz.vqdsnc.cn/gthruohyvx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtkhobitrj.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtrxvmtsoa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtgynilkhe.html

[R52] 统计行数
来源：http://hz.9152youxi.cn/gtogroxqpy.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtgssxougn.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtpbqpptll.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj20258888.top/gtzzrmemcp.html

[R54] 比较两个文件
来源：http://hz.hysaishi.cn/gtaelpzdzf.html

diff a.txt b.txt
来源：http://hz.bjfxy.top/gthxjctasg.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gttptylqdv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gthoeahtoh.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtjqwwygxs.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtpyyihvba.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtprevwdhb.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtqxyegmmq.html

[R58] 下载文件
来源：http://hz.aizwys.cn/gthzxpifwf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tianlin.xyz/gtbmpqjxro.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtfigpnumt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtjhdcrqsa.html

[R60] 只看 HTTP 状态码
来源：http://hz.aizwys.cn/gtrqhlrlph.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cheryme.top/gtuxtjandz.html

[R61] 磁盘占用
来源：http://hz.gotoacloud.top/gtyhxhjuzj.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gtuyuvhwic.html

[R62] 找最占空间的文件
来源：http://hz.zhaomingkeji.xyz/gtkixrzyri.html

du -ah . | sort -rh | head -10
来源：http://hz.hnxiangtu.top/gtksropcio.html

[R63] 内存与进程
来源：http://hz.smart0.xyz/gtoussayif.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gtifoefxsy.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtednsfdst.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenzaomai.com/gtdfntuhnj.html

[R65] 查看端口占用
来源：http://hz.hywenlv.cn/gtwgdjizbw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtdghpaqzu.html

[R66] 定时任务
来源：http://hz.zhiwuduotai.top/gtuhafmipf.html

crontab -e;  crontab -l
来源：http://hz.yuanzhike.top/gtzsldxzgr.html

[R67] 生成随机十六进制串
来源：http://hz.jqgfzy.top/gtzrubzusb.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gtxvqhsknk.html

[R68] 计算文件校验值
来源：http://hz.yonumen.top/gtahkjdtdw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pengpengdd.cyou/gtcdbxtzfq.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtxufofzkw.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtlieovkeb.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gtgexodtlz.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtsnqzklqt.html

[R71] 日期格式化
来源：http://hz.fzhhl.top/gthmznjcpj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gtewkybtmm.html

[R72] 等待端口就绪
来源：http://hz.andypj.xyz/gtyniqpifh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zycfv.cn/gtsfyngmnz.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtianuxypm.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gteqbewpfr.html

[R74] 批量重命名
来源：http://hz.haohaochexian.top/gtnkorkvfq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtfomfbpdp.html

[R75] 导出环境变量
来源：http://hz.aizwys.cn/gtupkpttpb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gtgulazavr.html

[R76] 使用临时文件
来源：http://hz.wangdashe.top/gtzunfnrlk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtptketccx.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gtdyfsliws.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtmswxadeo.html

[R78] 交互式菜单
来源：http://hz.hammf.cn/gtdyrxswaa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gthrsviwnq.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gtbcbqsoxy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gteqdczpys.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258888.top/gtliomfqdy.html

time ./run.sh
来源：http://hz.hnqzz.top/gtlxxyeyux.html

================================================================================
来源：http://hz.meibo888.top/gtfcltfatk.html

S. C / C++ 专题
来源：http://hz.cheryme.top/gtuoduinrf.html

================================================================================
来源：http://hz.aizwys.cn/gttwiyfwxv.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gttmzuvhvu.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtcacxrxku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtmrgzeoqt.html

[S02] C：变量与格式化输出
来源：http://hz.cashguo.top/gtonbehptw.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtcbpikqad.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtagbeadjm.html

int x; scanf("%d", &x);
来源：http://hz.birdmap.top/gtckeueefg.html

[S04] C：字符串复制
来源：http://hz.vqdsnc.cn/gtcamthayq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtwjhbkamy.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtdrgcsoln.html

strlen(s)
来源：http://hz.yueranfly.top/gtetaxlspo.html

[S06] C：字符串比较
来源：http://hz.pycfn.com/gtvvdrzsap.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtxvafpevl.html

[S07] C：数组遍历求和
来源：http://hz.cdnleiting.top/gtyqtmnywz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtuddhraji.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtzdlakzzb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gthzznejch.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gttzxbpyis.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtaqwwlazh.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtbfeukubh.html

int *p = &a;  *p = 5;
来源：http://hz.cheryme.top/gtinbjvqxd.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtzldziazb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.redwolf501.top/gteyqtktdm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtcnzcwpku.html

fclose(f);
来源：http://hz.316326.xyz/gtjxwukuqd.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtvvrwxtwe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtlqewnkpu.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtedatlvcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gtmpkpkvte.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtjlgldmzl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtorkawagw.html

[S15] C：类型转换
来源：http://hz.ydzc1.top/gtybzvfcik.html

(double) a / b
来源：http://hz.jinqigfzy.top/gtaemtsrqw.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtbnqutkqb.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtfqbdkzcx.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtutzjjfjy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cdnleiting.top/gthpbdwmeq.html

[S18] C：命令行参数
来源：http://hz.cqqwz.cn/gtqclfknyv.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gthsueqguf.html

[S19] C：快速排序
来源：http://hz.kuanghao11.cn/gtvvvhzmcj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gthfqsfqai.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtzjseirvn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtdrzrrqid.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gttjgtxbkr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtzbwuhgmg.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtofmoamzy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtlfktjlxs.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtzkucyuju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtmzxevylj.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtgkskiwfy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sweek.top/gtntkcpbic.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtqzzxiqsa.html

memcpy(dst, src, n);
来源：http://hz.zhaomingkeji.xyz/gtbutwduil.html

[S26] C：内存清零
来源：http://hz.yuanzhike.top/gtnsdslhgo.html

memset(a, 0, sizeof a);
来源：http://hz.zhiwuduotai.top/gtftqtqqkd.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtbrurhoaj.html

const double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtinspwkhl.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gthpnqsxzq.html

static int counter = 0;
来源：http://hz.zycfv.cn/gtbxnkasbe.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gtfqojsjhi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtxeldjnpm.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtpircoazu.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtouxfkxgq.html

#define X_H
来源：http://hz.hnxiangtu.top/gthnslpbwt.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtzhoddnhk.html

[S31] C++：Hello World
来源：http://hz.zhixingplan.top/gtschggplh.html

#include <iostream>
来源：http://hz.shangyingyoupin.top/gtnsjctymm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sufxvd.cn/gtwotsnvuu.html

[S32] C++：字符串
来源：http://hz.yongpay.top/gtxbtmgnwe.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtqbwttkkt.html

[S33] C++：vector 增删
来源：http://hz.ivvv.top/gtkmnvrrfc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hfpthk.cn/gtwlyntuyb.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtxapjuned.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtxthbhlyk.html

[S35] C++：map
来源：http://hz.yonumen.top/gtmpogxyai.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtipbvifkw.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtfqqmvnde.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtabznchgr.html

[S37] C++：set
来源：http://hz.xylfe.cn/gtbhxqepdj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtzwayzlbs.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gtjlidilsa.html

std::sort(v.begin(), v.end());
来源：http://hz.bjfxy.top/gtnjgavlsl.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gtdudyegxt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gtrksiaksf.html

[S40] C++：查找元素
来源：http://hz.quarkkingdee.top/gtypyfschh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.vqdsnc.cn/gtozfjgiep.html

[S41] C++：类与构造函数
来源：http://hz.yongpay.top/gtnaojgfal.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtzblfehkv.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gthsjiupak.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gtfiyrrbpy.html

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gtgtaijewx.html

auto p = std::make_unique<int>(5);
来源：http://hz.hongshengwenyu.top/gtakdmwewb.html

[S44] C++：引用传参
来源：http://hz.zycfv.cn/gtzokflucq.html

void inc(int &x) { ++x; }
来源：http://hz.0kj1m.cn/gtqwvvpgcu.html

[S45] C++：lambda
来源：http://hz.jiagoushi.top/gtyreqdkhc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtofdfgnys.html

[S46] C++：函数模板
来源：http://hz.yueranfly.top/gtcuyxtpyl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydzc1.top/gtyfxgccks.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj202588.top/gtwbhcapgp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtsojhlbdt.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gtirmaczpm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtfpjhspvr.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gtkqyslusg.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtspekutci.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.redwolf501.top/gtaclerlzl.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtrgksppww.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jiagoushi.top/gtyixxpxjo.html

[S51] C++：显式类型转换
来源：http://hz.dianchejie.cn/gtljlsoytx.html

static_cast<double>(a) / b
来源：http://hz.hammf.cn/gtmmkzcgoy.html

[S52] C++：const 与 noexcept
来源：http://hz.zhengqikj.top/gtmjftktxi.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigufen.top/gtfupxhsbl.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gtkkedemnt.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gtxrurvqdn.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gteigraylw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhengqikj.top/gtnygjptta.html

[S55] C++：结构化绑定
来源：http://hz.xinyue.icu/gteuppcfmz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuanzhike.top/gtygfqcgie.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtfyzpfbvq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jiagoushi.top/gtrtfzqryq.html

[S57] C++：编译期常量
来源：http://hz.gogol.net.cn/gtncxvfgyk.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtqjgmxtox.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtpmolsinz.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtntkngnyl.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtpiuaobgd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtrgkrjmcq.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtxuymqimz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.mhx1999.top/gtgpqqnqxc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gteummzdmh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gtuppfubaf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtetncpcus.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtognvwijk.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtgzyrxwpg.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtixaaybkx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtjzhjlvep.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtdnllxnfk.html

"值: $b"
来源：http://hz.gogol.net.cn/gtmqtlhfxe.html

[T04] Kotlin：空安全
来源：http://hz.shzxlz.cn/gtvocmyqwt.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gtktceqcep.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtnlpgeejv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtipxzxrmt.html

[T06] Kotlin：集合映射
来源：http://hz.gotoacloud.top/gtzilncdek.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tian-w.cn/gtgnxqcscf.html

[T07] Kotlin：集合过滤
来源：http://hz.ydjk.org.cn/gtvqiiosnv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guowangkeji.top/gticowjdgx.html

[T08] Kotlin：数据类
来源：http://hz.kuanghao11.cn/gttflsgrkc.html

data class User(val name: String, val age: Int)
来源：http://hz.bjfxy.top/gtltmqxooz.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtltixcsym.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtbyvbsizd.html

[T10] Kotlin：默认参数
来源：http://hz.shzxlz.cn/gtrvbfdqkk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtgffeueeo.html

[T11] Kotlin：协程
来源：http://hz.chenjidiqi.icu/gtjavfgquj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gtvjjzuziq.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtpfifjsvg.html

val (a, b) = Pair(1, 2)
来源：http://hz.quarkkingdee.top/gtxceazrpw.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtwvaxpvul.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gtatclvefc.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtnmghalni.html

for (i in 1..10) println(i)
来源：http://hz.vqdsnc.cn/gtrognfqua.html


<!-- 参考信息 -->