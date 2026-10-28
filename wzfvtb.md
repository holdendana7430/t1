代发 wailian999

[Q80] 字符串截取
来源：http://hz.sweek.top/gtklwmcach.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gogol.net.cn/gtcskguyxs.html

[Q81] 字符串替换
来源：http://hz.yj202588.top/gtoayyxudj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gtfdsztzcf.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gtycguiwdh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtdvitgvxe.html

[Q83] 大小写转换
来源：http://hz.cdnleiting.top/gtjchquhuw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gthkceolip.html

[Q84] 去除首尾空格
来源：http://hz.chenjidiqi.icu/gtiljlxzxj.html

SELECT TRIM(name) FROM users;
来源：http://hz.52xcode.cn/gtibnimkdl.html

[Q85] 数值取整
来源：http://hz.guowangkeji.top/gtbmepshcq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhongyouzk.top/gtekmfvcch.html

[Q86] 读取 JSON 字段
来源：http://hz.smart0.xyz/gtzrjzmxbz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtafuhhmko.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gtzmnnwkfv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gttwofdfce.html

[Q88] 行转列（条件聚合）
来源：http://hz.ywan-chungtsiang.top/gtpacycrtk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.birdmap.top/gtqowmwwvj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ehwqpu.com/gtvhehufay.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtizqlndyk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtllkcecjb.html

[Q90] 生成序号列
来源：http://hz.jiagoushi.top/gtqruytity.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtgbxwplgs.html

================================================================================
来源：http://hz.0kj1m.cn/gtxhmctcep.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gtmxtqorma.html

================================================================================
来源：http://hz.zdqjudy.top/gtquhkfaae.html

[R01] shebang 与严格模式
来源：http://hz.yuanzhike.top/gtvjwbtwvu.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtgpyqdxkd.html

set -euo pipefail
来源：http://hz.ppjwa.cn/gtunynfgdh.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtqrkcipnl.html

name="Tom"; echo "$name"
来源：http://hz.ybcxt.top/gtgyhkydpw.html

[R03] 只读变量
来源：http://hz.yonumen.top/gtycpouczx.html

readonly PI=3.14
来源：http://hz.ybcxt.top/gtwsmyabdm.html

[R04] 位置参数
来源：http://hz.daria6918.cn/gtzrqmurdu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.0kj1m.cn/gtgmdinzbr.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtmafegast.html

name="${1:-default}"
来源：http://hz.hammf.cn/gtkwukluvl.html

[R06] 判断命令是否存在
来源：http://hz.sxryk.cn/gtiwdhbhbx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aibaodan.cn/gtqvumpweu.html

[R07] if 判断文件
来源：http://hz.snrcjt.cn/gtaglkmhjj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhaomingkeji.xyz/gtylrbthwl.html

[R08] 数值比较
来源：http://hz.aibaodan.cn/gtdacpzwer.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtgfsinvkv.html

[R09] 字符串比较
来源：http://hz.cdnleiting.top/gtikakxmjm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yanxiufei.cn/gtzaxyrcbn.html

[R10] 正则匹配
来源：http://hz.yj20258888.top/gtwkcwhwln.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xziqi.cn/gtaomtdsgg.html

[R11] case 多分支
来源：http://hz.jlsjyb.cn/gtoocmducs.html

case "$1" in
来源：http://hz.ivvv.top/gtzlwjugif.html

start) echo "启动" ;;
来源：http://hz.zhaomingkeji.xyz/gtiemqrktn.html

stop)  echo "停止" ;;
来源：http://hz.jinghuilouyu.cn/gtwhtzlvdy.html

*)     echo "未知命令" ;;
来源：http://hz.cucudq.cn/gtepjvbkem.html

esac
来源：http://hz.pengpengdd.cyou/gtwgudxssk.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtuwlztggs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtfhsfzgyz.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtfppwubxz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhixingplan.top/gtedksrajo.html

[R14] C 风格 for
来源：http://hz.andypj.xyz/gtemfjccsu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtzbzbzpss.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtzyhxqifp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gttykjwhgw.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtfosmmbsz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtlceuhfpb.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtctoxonkm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtweutkqks.html

[R18] 遍历数组
来源：http://hz.vqdsnc.cn/gtygjxgfor.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hfpthk.cn/gtaggclvoe.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtedwkkfjs.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtvzdrwigm.html

[R20] 关联数组（字典）
来源：http://hz.aizwys.cn/gtdizfjxga.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jiagoushi.top/gtykvjmqwv.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gtrtnxmkox.html

echo "${#s}"
来源：http://hz.nwbrower.top/gtyggdwimw.html

[R22] 截取子串
来源：http://hz.wangshuangyany.cn/gtkffobybi.html

echo "${s:0:5}"
来源：http://hz.sxryk.cn/gtavqcoocw.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gtlhddxaen.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daria6918.cn/gtizldlwlu.html

[R24] 大小写转换
来源：http://hz.fzhhl.top/gtygnsztlg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtezinddhh.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxinkj.top/gtacezmqyj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtyabumlnf.html

[R26] 命令替换
来源：http://hz.yuxming.cn/gtozavsbmy.html

now=$(date +%F); echo "$now"
来源：http://hz.ppjwa.cn/gtimfbcled.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtrlfxljof.html

echo $((1 + 2 * 3))
来源：http://hz.cucudq.cn/gttpklwjew.html

[R28] 浮点运算
来源：http://hz.daxiang520.top/gtykrphhxj.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtgqevombr.html

[R29] 定义函数
来源：http://hz.ppjwa.cn/gtuaopikvz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ehwqpu.com/gtemdbrwxk.html

[R30] 函数返回状态码
来源：http://hz.dianchejie.cn/gtxyghyuqq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gtnoxugfao.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtilnavcoz.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtbpkhiglg.html

[R32] 参数个数校验
来源：http://hz.zhengqikj.top/gtotqoywlp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuxming.cn/gtltpqbuby.html

[R33] 捕获错误并提示行号
来源：http://hz.shuidangran.top/gtxcccewqb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aizwys.cn/gtbtrnvvji.html

[R34] 退出时清理
来源：http://hz.cucudq.cn/gtsibkjagt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtbpvnmvge.html

[R35] 后台执行并等待
来源：http://hz.zhijiandao.cn/gtperetnxl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ywan-chungtsiang.top/gtvkoezaex.html

[R36] 并发执行多个任务
来源：http://hz.ppjwa.cn/gtblurmakh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtbieikwnt.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtoqyfziiw.html

files=$(ls -1)
来源：http://hz.jinqigufen.top/gtyetvlbnm.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtbdwyemor.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fengsongda.top/gtcbmcdvke.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtuahcyjee.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtmmjgrrsd.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtzkxgyvjy.html

echo "log" >> out.log
来源：http://hz.yuanzhike.top/gtfsdxxqto.html

[R41] 丢弃输出
来源：http://hz.jinqigufen.top/gtlvtvairj.html

cmd >/dev/null 2>&1
来源：http://hz.zhixingplan.top/gtgrxeghmq.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtqzdpusus.html

wc -l < a.txt
来源：http://hz.zhoulong.xyz/gtidmyryrp.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtkgvhgjrd.html

find . -name "*.log" -type f
来源：http://hz.chenjidiqi.icu/gtywdjbhfo.html

[R44] 按修改时间查找
来源：http://hz.ppjwa.cn/gtgugjrjxn.html

find . -mtime -7 -type f
来源：http://hz.chenzaomai.com/gtvopvclrk.html

[R45] 批量删除
来源：http://hz.316326.xyz/gtlofjaoyl.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gtpoogneuq.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gttonkqxah.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gteacmsmbz.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtwsyrpyvu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.0kj1m.cn/gtxyqzvdjm.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtcsdmmfuw.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtcwtqwzrt.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtmrqcrnck.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gttdcjawzh.html

[R50] awk 求和
来源：http://hz.zhoulong.xyz/gtcuiaoijc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigfzy.top/gtjomqyiim.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtbuasjrwb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sxryk.cn/gtzvqxirqw.html

[R52] 统计行数
来源：http://hz.hnxiangtu.top/gtmlkdwnrg.html

wc -l a.txt
来源：http://hz.hammf.cn/gtfxhutund.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtrkxxytzp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtksxxhjpx.html

[R54] 比较两个文件
来源：http://hz.jinqigufen.top/gtqxmxnrlm.html

diff a.txt b.txt
来源：http://hz.hongshengwenyu.top/gtlcpxqwur.html

[R55] 压缩与解压
来源：http://hz.ydzc1.top/gtvzqxldpu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.iojbl.cn/gtbodmygpo.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gthdccszkb.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtwxecbalc.html

[R57] 远程执行命令
来源：http://hz.yonumen.top/gtwpvmqvrv.html

ssh user@host 'uptime'
来源：http://hz.pengpengdd.cyou/gtczkbkfol.html

[R58] 下载文件
来源：http://hz.xingfuxueyuan.xyz/gtlbrzqvtg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gthzvygjrc.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtopkgohcm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtjfjvznts.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gttwocsqya.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pycfn.com/gteamhuoaz.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtlzypqvdy.html

df -h;  du -sh *
来源：http://hz.yuanzhike.top/gtuskkhpbs.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtjahhykpc.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gtplandlqz.html

[R63] 内存与进程
来源：http://hz.dianchejie.cn/gtattobvww.html

free -h;  ps aux | grep nginx
来源：http://hz.0kj1m.cn/gtipeoiejb.html

[R64] 结束进程
来源：http://hz.aibaodan.cn/gtqhorwito.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tianlin.xyz/gtageobjzb.html

[R65] 查看端口占用
来源：http://hz.sysykeji.top/gtxbzteahw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtvcxuiczu.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtdmfwypsz.html

crontab -e;  crontab -l
来源：http://hz.jinghuilouyu.cn/gtacbxgxuh.html

[R67] 生成随机十六进制串
来源：http://hz.aizwys.cn/gtjgojdkuo.html

openssl rand -hex 16
来源：http://hz.vqdsnc.cn/gtqfoeyrmg.html

[R68] 计算文件校验值
来源：http://hz.cheryme.top/gtnvykkrjw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtgowfeebh.html

[R69] 生成随机密码
来源：http://hz.xziqi.cn/gtyhixoggo.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtlcnsbxoa.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtciunhhoc.html

date +%s;  date -d @1700000000
来源：http://hz.0kj1m.cn/gtyvzgfutw.html

[R71] 日期格式化
来源：http://hz.nanxuanxn.top/gthavjxyss.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nwbrower.top/gtwpbfrggs.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtalsynowo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtprqrwafq.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtigtsxcok.html

split -l 1000 big.log part_
来源：http://hz.ppjwa.cn/gtnbryrxld.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtjownntsx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ydjk.org.cn/gtcbmbtifc.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtyboiwupg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinghuilouyu.cn/gthhfvnvfx.html

[R76] 使用临时文件
来源：http://hz.guannengcc.top/gtdclghkku.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gtnziewrlr.html

[R77] 读取用户输入
来源：http://hz.redwolf501.top/gtysudlkho.html

read -rp "请输入: " ans
来源：http://hz.zdqjudy.top/gtjmaxbtpj.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtvbhbvldr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangshuangyany.cn/gturhcjxgu.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtgnjfggds.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtjqubavgc.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtbazfccxg.html

time ./run.sh
来源：http://hz.aizwys.cn/gtiryvwfcf.html

================================================================================
来源：http://hz.guannengcc.top/gtptbnbedj.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtzhiochud.html

================================================================================
来源：http://hz.jlsjyb.cn/gtauiljqdb.html

[S01] C：Hello World
来源：http://hz.xuetiantiany.cn/gtdgznoxxt.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtmqgaxbeo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gteoibiehx.html

[S02] C：变量与格式化输出
来源：http://hz.xziqi.cn/gtorhngjpa.html

int a = 10; printf("%d\n", a);
来源：http://hz.yvedp.cn/gtnlgwnkwt.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtbttizlry.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtlzdghpzc.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtvazlpqfy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtaqotjasq.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtaulhffju.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtzrunbzxz.html

[S06] C：字符串比较
来源：http://hz.wangshuangyany.cn/gtrimjbyri.html

strcmp(a, b) == 0
来源：http://hz.zycfv.cn/gtsusgxtih.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtcbirclgp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtkuhjjgpy.html

[S08] C：动态内存分配与释放
来源：http://hz.nwbrower.top/gtngmfzhvs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gtxjigxhpc.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gtduvukopn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shuidangran.top/gtkiewidil.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtfwzufnyf.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gttuiewabx.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtbqoxlefp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtwputrfxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtlxwigpwz.html

fclose(f);
来源：http://hz.yj20258.top/gtptjdcsoo.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtvkoujizk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtbjqcramk.html

[S13] C：宏定义
来源：http://hz.cqqwz.cn/gtyaoxdjvb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtpkfgeigp.html

[S14] C：枚举
来源：http://hz.sysykeji.top/gtovtbfypt.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gtvyfgwgdj.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gthrarkyoz.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtehonlcvq.html

[S16] C：位操作置位
来源：http://hz.yongpay.top/gtkwrecqex.html

x |= (1 << 3);
来源：http://hz.birdmap.top/gtswqfgjnh.html

[S17] C：安全拼接字符串
来源：http://hz.xuanzx.com/gtrqbkqcng.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtbmiafmwz.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtmbhqdnkf.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtwgtowonw.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gttpgqnzsq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gttacnfcjy.html

[S20] C：二分查找
来源：http://hz.mhx1999.top/gtzzpzynyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtofyajpfq.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gtfukryzrx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtmysngwua.html

[S22] C：字符串转数字
来源：http://hz.sufxvd.cn/gtcozbnpcc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daria6918.cn/gtkgcfmvev.html

[S23] C：随机数
来源：http://hz.redwolf501.top/gtpdaafybl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtutjqovjo.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtgfmhpcuv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtqzbkhinf.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangkeji.top/gthcyerodj.html

memcpy(dst, src, n);
来源：http://hz.xuanzx.com/gtnmrtlmgl.html

[S26] C：内存清零
来源：http://hz.hysaishi.cn/gtcsfmgcrr.html

memset(a, 0, sizeof a);
来源：http://hz.tian-w.cn/gtmmiznatm.html

[S27] C：定义常量
来源：http://hz.andypj.xyz/gtoblzakgi.html

const double PI = 3.14159;
来源：http://hz.iojbl.cn/gtgxuuntkv.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtbmggarpc.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtrndswyzk.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gthsgntxgz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtkaqbplnd.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtidgefqsl.html

#ifndef X_H
来源：http://hz.feifeiyinyue.top/gtnheboahu.html

#define X_H
来源：http://hz.hnqzz.top/gtgustbycf.html

#endif
来源：http://hz.hfpthk.cn/gtaxkqpteb.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtvppubfli.html

#include <iostream>
来源：http://hz.tanke756.top/gtejsemslr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtoqgzkkhn.html

[S32] C++：字符串
来源：http://hz.sweek.top/gtaupicpyq.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtdtltolii.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtimrwjoco.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtqpeczwrs.html

[S34] C++：遍历 vector
来源：http://hz.snrcjt.cn/gtkmkbsban.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtpanvfzjc.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtccwtmyvo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtyodsjejp.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtebzvlzdr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtagnjartb.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gttsykneyp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.mhx1999.top/gtmuujmxau.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtgcfrmjdc.html

std::sort(v.begin(), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtviefgvni.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtpokfflbz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.bjfxy.top/gtwrtwjjug.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtxsditsqa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhengqikj.top/gtlqenvtwp.html

[S41] C++：类与构造函数
来源：http://hz.mhx1999.top/gtfnutldqn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtvbloghbi.html

[S42] C++：继承与虚函数
来源：http://hz.iojbl.cn/gtxwbsoydk.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gthvkhnqqp.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtyuopmbep.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtztejxaec.html

[S44] C++：引用传参
来源：http://hz.daxiang520.top/gtlfzsacsx.html

void inc(int &x) { ++x; }
来源：http://hz.guannengcc.top/gtwwpybfro.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtzyineqke.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtbuzdlbfc.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtjrhpakei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtgkfvyurn.html

[S47] C++：结构化绑定遍历
来源：http://hz.gotoacloud.top/gtxiwwtits.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.meibo888.top/gtwsykeiss.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gthfvczwjn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hammf.cn/gtwqzgtsja.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gttyefizfg.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtbsxrzdlq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtfmscamnt.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gturhhsqqz.html


<!-- 参考信息 -->