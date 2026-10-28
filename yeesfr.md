代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gthgpufzda.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gttvbosoxh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gtvqitfgrm.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gttgohrwfo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangdashe.top/gtwahnzuds.html

[R18] 遍历数组
来源：http://hz.yongpay.top/gtasjwfszp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dianchejie.cn/gtdzfhrxpk.html

[R19] 数组长度
来源：http://hz.feifeiyinyue.top/gtzrsfmdnp.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtyhnafaqe.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtqqtlrlen.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuanzhike.top/gtgjcgbfid.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gtcxhtecdv.html

echo "${#s}"
来源：http://hz.yvedp.cn/gtzaquxnhz.html

[R22] 截取子串
来源：http://hz.c1oappe.top/gtrprdnwmu.html

echo "${s:0:5}"
来源：http://hz.zhengqikj.top/gtwhfijveu.html

[R23] 字符串替换
来源：http://hz.hnxiangtu.top/gtoqvenwtv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtrpteehur.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtbunofveo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shuidangran.top/gtydssmwlw.html

[R25] 去后缀 / 去前缀
来源：http://hz.vqdsnc.cn/gtcgmaflkj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zycfv.cn/gtajmadhmy.html

[R26] 命令替换
来源：http://hz.tian-w.cn/gtjaefziaw.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtfxbxqqcq.html

[R27] 算术展开
来源：http://hz.shanyushiyangtech.top/gtaqfvkibc.html

echo $((1 + 2 * 3))
来源：http://hz.jyoumei.cn/gturlfossu.html

[R28] 浮点运算
来源：http://hz.xuetiantiany.cn/gtdvatwipr.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtkkicnddt.html

[R29] 定义函数
来源：http://hz.hammf.cn/gtomluuymq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangkeji.top/gtwanybzkx.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtpgvsiiee.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gtslbssxcy.html

[R31] 局部变量
来源：http://hz.9152youxi.cn/gtmblizhwp.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtfticjqoi.html

[R32] 参数个数校验
来源：http://hz.zhoulong.xyz/gtwpcheehh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gthwxqztnc.html

[R33] 捕获错误并提示行号
来源：http://hz.jianghu66.top/gtroxlqryu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenzaomai.com/gtlyzqjsem.html

[R34] 退出时清理
来源：http://hz.gaohongyu789.top/gtqppalwrk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gttuikdzee.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtxnycymeq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cashguo.top/gtuxtxktrn.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtrurljyna.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.birdmap.top/gtrpgmvmgc.html

[R37] 把输出赋给变量
来源：http://hz.jqgfzy.top/gtufnyhbhf.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtpnytwsrs.html

[R38] 管道串联
来源：http://hz.wangshuangyany.cn/gtxeoijefj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.andypj.xyz/gtofhvdsvm.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtqrxrceyu.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtiewppejc.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtgtgzzdgz.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtaaiwlzes.html

[R41] 丢弃输出
来源：http://hz.chenlongwang.top/gtdeopmxtx.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gtvjqybixt.html

[R42] 输入重定向
来源：http://hz.gaohongyu789.top/gthvcnpwbk.html

wc -l < a.txt
来源：http://hz.chenlongwang.top/gtzajxgagn.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtxgezscle.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtfiqwgphb.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gtyeilslor.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtqlyabset.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtdpopygyu.html

find . -name "*.tmp" -delete
来源：http://hz.hnxiangtu.top/gtitjbwong.html

[R46] 递归替换文件内容
来源：http://hz.zhixingplan.top/gtgwcfuksp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dianchejie.cn/gtclilxobb.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtzrsbpggs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jiagoushi.top/gtdhlxebbv.html

[R48] awk 取指定列
来源：http://hz.jlsjyb.cn/gtqdfdulln.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnxiangtu.top/gtqicubouf.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtavgmmxie.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangshuangyany.cn/gtgirqudvp.html

[R50] awk 求和
来源：http://hz.hywenlv.cn/gtnwgxtnov.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pengpengdd.cyou/gtjivnemhc.html

[R51] 排序去重取前几
来源：http://hz.0kj1m.cn/gtcgbymigq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cqqwz.cn/gtdbnrcolc.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtvipnwnvd.html

wc -l a.txt
来源：http://hz.yj202588.top/gtilxmkizp.html

[R53] 查看文件头与实时尾
来源：http://hz.hfpthk.cn/gtosmdeltq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nwbrower.top/gttonknpin.html

[R54] 比较两个文件
来源：http://hz.haohaochexian.top/gtjgmigkpp.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gttbngkwzq.html

[R55] 压缩与解压
来源：http://hz.9152youxi.cn/gtccrqrkrc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.52xcode.cn/gtmhfddakp.html

[R56] 远程拷贝
来源：http://hz.wangshuangyany.cn/gtkkdljyjk.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtntyaxdzu.html

[R57] 远程执行命令
来源：http://hz.hongshengwenyu.top/gtufypclnr.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtqmqxexyx.html

[R58] 下载文件
来源：http://hz.jinyuanbaomall.cn/gtxsvfntgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtrpdjzeok.html

[R59] 发 POST JSON
来源：http://hz.aizwys.cn/gtwxowutbn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hywenlv.cn/gtevexsqjt.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258.top/gtpstvzzne.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gtenylsomb.html

[R61] 磁盘占用
来源：http://hz.tian-w.cn/gtkgotfzzf.html

df -h;  du -sh *
来源：http://hz.sufxvd.cn/gtkdqcinvk.html

[R62] 找最占空间的文件
来源：http://hz.gogol.net.cn/gtymwipebq.html

du -ah . | sort -rh | head -10
来源：http://hz.sufxvd.cn/gtwbarstoc.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gteacfmoux.html

free -h;  ps aux | grep nginx
来源：http://hz.quarkkingdee.top/gtvpjcsleb.html

[R64] 结束进程
来源：http://hz.ehwqpu.com/gttlnjptzh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gotoacloud.top/gtgmnqghhw.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gtzxyajkfw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gogol.net.cn/gtpplyyjhw.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtifgazgbb.html

crontab -e;  crontab -l
来源：http://hz.xingfuxueyuan.xyz/gtqidwmsww.html

[R67] 生成随机十六进制串
来源：http://hz.aibaodan.cn/gtvkedacsu.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtfklpekti.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtwmtvmclp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnqzz.top/gtniztpvpa.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtlnpiovci.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtrkluielr.html

[R70] 时间戳与互转
来源：http://hz.ybcxt.top/gtnnrvkhfq.html

date +%s;  date -d @1700000000
来源：http://hz.guowangkeji.top/gtfyisbvsf.html

[R71] 日期格式化
来源：http://hz.guannengcc.top/gtqekajryj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aibaodan.cn/gtannklwzp.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtpryzpryl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.9152youxi.cn/gtzpvyrlkr.html

[R73] 分割大日志
来源：http://hz.tianlin.xyz/gthmcfkjix.html

split -l 1000 big.log part_
来源：http://hz.cashguo.top/gtyntwrhjw.html

[R74] 批量重命名
来源：http://hz.ywan-chungtsiang.top/gtqfouwhdf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.52xcode.cn/gtfuuertqb.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtnjzhqboq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhaomingkeji.xyz/gtkditdnsb.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtaprgaupx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtcqfgutqs.html

[R77] 读取用户输入
来源：http://hz.hongshengwenyu.top/gthawequsx.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gthehtmbna.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gttqgirkbx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gthoxvnrdq.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtyjmvxvhn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtfgzmpicn.html

[R80] 查看脚本执行耗时
来源：http://hz.vqdsnc.cn/gtzgupyvrp.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtgvtzofxo.html

================================================================================
来源：http://hz.aibaodan.cn/gtcbfvmgzl.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtokqyvkyy.html

================================================================================
来源：http://hz.fengsongda.top/gtfthgatpa.html

[S01] C：Hello World
来源：http://hz.hnxiangtu.top/gtkgdhpuys.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtthbvneqx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangshuangyany.cn/gtopyzctnm.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtfsvryhkk.html

int a = 10; printf("%d\n", a);
来源：http://hz.pycfn.com/gtxydrszaa.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gtjohjhicl.html

int x; scanf("%d", &x);
来源：http://hz.nanxuanxn.top/gtazbmskqt.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gtggwclmqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtnhcfpvit.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gtcpzvxcmi.html

strlen(s)
来源：http://hz.chenzaomai.com/gtgqnsosbn.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtfrfcwfwy.html

strcmp(a, b) == 0
来源：http://hz.gotoacloud.top/gticvhherh.html

[S07] C：数组遍历求和
来源：http://hz.tianlin.xyz/gtwhohxysj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtbutlpwqs.html

[S08] C：动态内存分配与释放
来源：http://hz.kuanghao11.cn/gtjsisepja.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.havefunace.top/gtzrlcgbil.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtixnknooq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gtdbmfuutx.html

[S10] C：指针与解引用
来源：http://hz.zhongyouzk.top/gtciufqgxx.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtmebyflbl.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtceevoahu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.haohaochexian.top/gtbqmbpkkt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgfzy.top/gttcttiueo.html

fclose(f);
来源：http://hz.fzhhl.top/gtnvdwaabt.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtvhnepwul.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtotvdjcuf.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtahososmd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gtjfgmahby.html

[S14] C：枚举
来源：http://hz.nwbrower.top/gtoafgniqu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtenagjtve.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtwqmnnjya.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtxwmllqas.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gtgmtkoikh.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtrvohhooj.html

[S17] C：安全拼接字符串
来源：http://hz.yanxiufei.cn/gtsevlpgqq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtzyzagmlh.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtghntkuxx.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gtuvqnuxnj.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtioofjwzd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtmjqpghyy.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtnkikmziq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtqkeaofdi.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtytrmhihs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtqpnzyuml.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtzwqtneed.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtwxfyertm.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtgahzgkwa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gtxuwwboqe.html

[S24] C：获取本地时间
来源：http://hz.vqdsnc.cn/gtxiricevg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtlveytrjr.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gtysariwgd.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtrhvqebov.html

[S26] C：内存清零
来源：http://hz.shuidangran.top/gtekehyqio.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gthsyqvida.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gtjynzelve.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtltkmzeeg.html

[S28] C：静态变量
来源：http://hz.kuanghao11.cn/gtauhojdqi.html

static int counter = 0;
来源：http://hz.ppjwa.cn/gtaxztbgqk.html

[S29] C：变参函数
来源：http://hz.smart0.xyz/gtvtkugwog.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gtizpwhrwr.html

[S30] C：头文件保护
来源：http://hz.yj20258888.top/gtprmzxukp.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gtfgowzqfy.html

#define X_H
来源：http://hz.smart0.xyz/gtqvitwuin.html

#endif
来源：http://hz.yj20258.top/gtbzjtllks.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtdpthskmm.html

#include <iostream>
来源：http://hz.xuetiantiany.cn/gtmezkojmm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xylfe.cn/gtqnvglgrw.html

[S32] C++：字符串
来源：http://hz.cdnleiting.top/gtuzazyiwi.html

std::string s = "hi";  s += "!";
来源：http://hz.zhongyouzk.top/gtukridguc.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtaukragwo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtlqgtncra.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtgcjepbtb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtrzxmkddm.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtrrmuoiqa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtnsniaewl.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtsmnhpzau.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtpwajezwv.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtqbimjqkx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zycfv.cn/gtabhclnxr.html

[S38] C++：排序
来源：http://hz.yj202588.top/gtnscyomjy.html

std::sort(v.begin(), v.end());
来源：http://hz.svipenyu.cn/gtzvmmdsoj.html

[S39] C++：自定义比较器排序
来源：http://hz.ppjwa.cn/gtmbbwqxcs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtojchbgaj.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtrrkcdplx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtaryfolbu.html

[S41] C++：类与构造函数
来源：http://hz.mhx1999.top/gthzuoemuv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtpggjgldw.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtxatdrjta.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtnaoptqpa.html

[S43] C++：智能指针
来源：http://hz.yonumen.top/gtqhntsxom.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gtgrvmtafv.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtatwpfjfj.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtjghapmsn.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtjwsnoboa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtfkpuheit.html

[S46] C++：函数模板
来源：http://hz.hnqzz.top/gtpvaiycim.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtftxtsjfl.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinghuilouyu.cn/gttkwjhvhn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenlongwang.top/gtmydwbzyy.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gtpshjjvve.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtaykpdcsp.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gteqqroydm.html

[S49] C++：写文件
来源：http://hz.jlsjyb.cn/gtbtksdfax.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtkhxrkmrt.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtpmtpktzq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtuzxxynik.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtlpexhlao.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtkjqxidid.html

[S52] C++：const 与 noexcept
来源：http://hz.shangyingyoupin.top/gtuqswejpd.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtexkbeosy.html

[S53] C++：移动语义
来源：http://hz.9152youxi.cn/gtjhgybfyd.html

std::vector<int> w = std::move(v);
来源：http://hz.quarkkingdee.top/gtevzkouki.html

[S54] C++：异常处理
来源：http://hz.hfpthk.cn/gtyamxkitm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jianghu66.top/gturfehuzx.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtqbblqyin.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtqlchiqjc.html

[S56] C++：optional
来源：http://hz.fengsongda.top/gtcmapdfiv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sysykeji.top/gtmqxwjpmq.html

[S57] C++：编译期常量
来源：http://hz.jinqigufen.top/gthawfkfty.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtuufaklnj.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gtrdktedwk.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gttccemctd.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtvvljlydi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.andypj.xyz/gtsgorvexp.html

[S60] C++：遍历并删除元素
来源：http://hz.hammf.cn/gtwnuosmuq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtaahwkkrp.html

================================================================================
来源：http://hz.zhengqikj.top/gtsmkoxqbb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtktkrjsou.html

================================================================================
来源：http://hz.jiagoushi.top/gtgixofssy.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gtuputvkuy.html

println("Hello")
来源：http://hz.hywenlv.cn/gthmtqsvsq.html

[T02] Kotlin：变量
来源：http://hz.dianchejie.cn/gtgqdnjcab.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtlvulqosr.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtwzfoealt.html

"值: $b"
来源：http://hz.kuanghao11.cn/gterasopdi.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gteqcgqcks.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangtech.top/gttyvlgvev.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtkeeverig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtvcujtycy.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtmtfoiygo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gteyizyfnj.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtxyqtxbbc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtnaywnjns.html

[T08] Kotlin：数据类
来源：http://hz.c1oappe.top/gtrxjyhuia.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtjjhscdat.html

[T09] Kotlin：扩展函数
来源：http://hz.dianchejie.cn/gtlzuhkmbx.html

fun String.exclaim() = this + "!"
来源：http://hz.ydjk.org.cn/gtdwsxoaof.html

[T10] Kotlin：默认参数
来源：http://hz.havefunace.top/gtmmtxdfbc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtgqbhmvjr.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtqodrbuvm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtciusocno.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtidvyieqv.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gtaeyjqhll.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gtyheogzuz.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gtvmbfyvkn.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtuvwrmzju.html

for (i in 1..10) println(i)
来源：http://hz.feifeiyinyue.top/gtihvaggii.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtkpxnacok.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gtzxrawksh.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gtjfdceeet.html

print("Hello")
来源：http://hz.sxryk.cn/gtyvdsghqi.html

[T17] Swift：变量与常量
来源：http://hz.xingfuxueyuan.xyz/gtujkbeqln.html

var a = 1;  let b = 2
来源：http://hz.ppjwa.cn/gtmehwhkoc.html

[T18] Swift：字符串插值
来源：http://hz.zhiwuduotai.top/gtmysgnngo.html

"值: \(b)"
来源：http://hz.jinqigufen.top/gtkmvjblly.html


<!-- 参考信息 -->