代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtrnrdvgrb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtpiqnwmxb.html

[Q87] JSON 字段做条件
来源：http://hz.xinyue.icu/gtqkfnxjce.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtscaqvwrt.html

[Q88] 行转列（条件聚合）
来源：http://hz.shuidangran.top/gtdsnfpbgw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ppjwa.cn/gtyljoudci.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtpfhlssyi.html

[Q89] 判断表是否存在
来源：http://hz.yj202588.top/gtjjqknuma.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tian-w.cn/gtfzelvcbo.html

[Q90] 生成序号列
来源：http://hz.feifeiyinyue.top/gtzonqgcjf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtjxmrwwam.html

================================================================================
来源：http://hz.tianlin.xyz/gtbovrpufs.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtrioqrqjw.html

================================================================================
来源：http://hz.aizwys.cn/gttxgfbtob.html

[R01] shebang 与严格模式
来源：http://hz.iojbl.cn/gtoymhyvwb.html

#!/usr/bin/env bash
来源：http://hz.jinqigfzy.top/gtggfvtwqj.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtyhdluqpj.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtqmvnknqr.html

name="Tom"; echo "$name"
来源：http://hz.yonumen.top/gtibaojpvf.html

[R03] 只读变量
来源：http://hz.sxryk.cn/gtqynmvdxt.html

readonly PI=3.14
来源：http://hz.tianlin.xyz/gtuvsrwclc.html

[R04] 位置参数
来源：http://hz.jinghuilouyu.cn/gtxwiitxvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jianghu66.top/gtnsoiqlet.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtlsprklkp.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtpsduemff.html

[R06] 判断命令是否存在
来源：http://hz.xinyue.icu/gtceeegqtm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtngynihoi.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gtajbuizzi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhongyouzk.top/gtolexasaf.html

[R08] 数值比较
来源：http://hz.hysaishi.cn/gtjqtpfenu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtpviyrtnt.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtrbpovrxs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xingfuxueyuan.xyz/gtnefcdxhg.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtkzngavbb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.svipenyu.cn/gtqxognlaq.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtljkoktwx.html

case "$1" in
来源：http://hz.fzhhl.top/gtvgsacvgx.html

start) echo "启动" ;;
来源：http://hz.gotoacloud.top/gtlvbdlbvq.html

stop)  echo "停止" ;;
来源：http://hz.fzhhl.top/gtbrduzzkl.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtajcvseiy.html

esac
来源：http://hz.zhoulong.xyz/gtcgvtuxau.html

[R12] for 遍历文件
来源：http://hz.9152youxi.cn/gtwocijicc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinyuanbaomall.cn/gtrtawthgp.html

[R13] for 计数循环
来源：http://hz.jinqigufen.top/gtensovwel.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gtcjmxnvgm.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtawrrgtjk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtoawrpatj.html

[R15] while 逐行读文件
来源：http://hz.nanxuanxn.top/gtzkaaecdl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtnffwgjon.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtbgteyuit.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aibaodan.cn/gtvgznoyld.html

[R17] 数组定义与取值
来源：http://hz.sweek.top/gtijgemysj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtsmwsijze.html

[R18] 遍历数组
来源：http://hz.ivvv.top/gtbixraeiy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtxidxyejd.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtawgqejfo.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gttjodltep.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtroyyovrb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gthavkhcpl.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gtpsnclazv.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtbamkquex.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtnphlkkgu.html

echo "${s:0:5}"
来源：http://hz.ydjk.org.cn/gtgqgzwagx.html

[R23] 字符串替换
来源：http://hz.jinqigufen.top/gtkmhavdje.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtmpjqjddm.html

[R24] 大小写转换
来源：http://hz.havefunace.top/gtypnizuts.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xylfe.cn/gtdgrvkpif.html

[R25] 去后缀 / 去前缀
来源：http://hz.jlsjyb.cn/gtkjgolpfu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtylkdnajm.html

[R26] 命令替换
来源：http://hz.xuanzx.com/gtnikdbwkg.html

now=$(date +%F); echo "$now"
来源：http://hz.chenzaomai.com/gtpedlkjfr.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtkzxjqaaa.html

echo $((1 + 2 * 3))
来源：http://hz.c1oappe.top/gtbihkseda.html

[R28] 浮点运算
来源：http://hz.yuanzhike.top/gtstbsydca.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258888.top/gthtupkwls.html

[R29] 定义函数
来源：http://hz.jqgfzy.top/gtqinmrerd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ybcxt.top/gthnnvgfjp.html

[R30] 函数返回状态码
来源：http://hz.smart0.xyz/gtwmrcskxz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gttvbrjkkn.html

[R31] 局部变量
来源：http://hz.jinghuilouyu.cn/gtvoqmicin.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gttwwsrbzd.html

[R32] 参数个数校验
来源：http://hz.yueranfly.top/gtifdahfkk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtthiakhbj.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtyoxrkwsr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aizwys.cn/gtzoxcekwy.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtxupdhctr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtnbxiecns.html

[R35] 后台执行并等待
来源：http://hz.shzxlz.cn/gtqkimxerq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.iojbl.cn/gtfwtkwtbp.html

[R36] 并发执行多个任务
来源：http://hz.gotoacloud.top/gtdycoamrv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ydzc1.top/gtteybpjsr.html

[R37] 把输出赋给变量
来源：http://hz.cucudq.cn/gtppemoxqw.html

files=$(ls -1)
来源：http://hz.hysaishi.cn/gtvxsdteaz.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtaxfvitjm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtqslnywnl.html

[R39] 重定向标准输出与错误
来源：http://hz.quarkkingdee.top/gtzqenyugx.html

cmd > out.log 2>&1
来源：http://hz.zhongyouzk.top/gtbzvxhrsf.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gtlwglhqmz.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtifbhmccv.html

[R41] 丢弃输出
来源：http://hz.zhengqikj.top/gtrofrhhzl.html

cmd >/dev/null 2>&1
来源：http://hz.yueranfly.top/gtnapmhzom.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gthjvtliwh.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gtidsajjwd.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtdgjodolt.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtxlmcfhzt.html

[R44] 按修改时间查找
来源：http://hz.redwolf501.top/gtghhlsrnp.html

find . -mtime -7 -type f
来源：http://hz.shuidangran.top/gtfuznmdpa.html

[R45] 批量删除
来源：http://hz.yj20258.top/gtqibcrbte.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtszucyjhw.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtheqlgeiz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yueranfly.top/gtgmcdunto.html

[R47] sed 单行替换
来源：http://hz.nwbrower.top/gtxfhnpide.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtouucooal.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtfhpdoprv.html

awk '{print $1, $3}' a.txt
来源：http://hz.hfpthk.cn/gtjhxqnrpv.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtoqazhsre.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtbrojwlnf.html

[R50] awk 求和
来源：http://hz.sufxvd.cn/gtwynpucgb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtbsjtqgcc.html

[R51] 排序去重取前几
来源：http://hz.zhoulong.xyz/gtegusgeuh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtzkwoskvz.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtcoqhnjvz.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtaqljyvju.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtfgjzsvjn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtchqtzrfr.html

[R54] 比较两个文件
来源：http://hz.yuanzhike.top/gtikllsrbd.html

diff a.txt b.txt
来源：http://hz.jinqigufen.top/gtkpmxoeoh.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtzyisxyoj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gttaupcwps.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtwkdowpuv.html

scp file user@host:/path/
来源：http://hz.wangshuangyany.cn/gtgnssnqht.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtvssjhaki.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtxebtnbig.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gtuptgtukd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtrthmgmpt.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtbmhsroox.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtrsumxnsi.html

[R60] 只看 HTTP 状态码
来源：http://hz.yangfankeji.com/gtgkuudupe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.9152youxi.cn/gtkwyaexxk.html

[R61] 磁盘占用
来源：http://hz.hfpthk.cn/gtqkbdrpnu.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gtfmtfozjx.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtsllodsam.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtxuggzkjq.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtuydgbwnp.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtjjwrrzto.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtqsflgdtn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtvlpsdrbj.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtxzaimsyn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.bjfxy.top/gtndkdxlxa.html

[R66] 定时任务
来源：http://hz.birdmap.top/gttrqnbyyu.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtdldqcgqh.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtvntouoqh.html

openssl rand -hex 16
来源：http://hz.zdqjudy.top/gtcgrvtmhc.html

[R68] 计算文件校验值
来源：http://hz.wangdashe.top/gtmsgndiek.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtegteinun.html

[R69] 生成随机密码
来源：http://hz.zhoulong.xyz/gtfgvjukxt.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtgnncydfu.html

[R70] 时间戳与互转
来源：http://hz.bjfxy.top/gtskgkeuzu.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtmodwgndu.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtujaejryx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sxryk.cn/gtrsfhrpmk.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtllsbnqvi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.smart0.xyz/gtkczomwzb.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtwvgrupjt.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtknxgblqe.html

[R74] 批量重命名
来源：http://hz.cashguo.top/gtcpndqoot.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gtcnylklzj.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtoiyrjzaj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtpcbqokfj.html

[R76] 使用临时文件
来源：http://hz.yj20258888.top/gtezmmnnqo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtpxgmcbos.html

[R77] 读取用户输入
来源：http://hz.havefunace.top/gtudkijvyz.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtumixezvc.html

[R78] 交互式菜单
来源：http://hz.shuidangran.top/gtydlrwwdx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gthcbsrerl.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtxjwsydsb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhongyouzk.top/gtyzwbiyca.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtysicecwx.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtxzfpcfwp.html

================================================================================
来源：http://hz.sufxvd.cn/gtzhclqnfw.html

S. C / C++ 专题
来源：http://hz.tanke756.top/gtxrrcbpji.html

================================================================================
来源：http://hz.nwbrower.top/gtrsnwomts.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtvdzjyivr.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtkxxihorw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cashguo.top/gtrmlzbtny.html

[S02] C：变量与格式化输出
来源：http://hz.ehwqpu.com/gtwrgfwmam.html

int a = 10; printf("%d\n", a);
来源：http://hz.0kj1m.cn/gtslbkfxcv.html

[S03] C：读入整数
来源：http://hz.haohaochexian.top/gtyidtyhuo.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gtctcqbrgl.html

[S04] C：字符串复制
来源：http://hz.smart0.xyz/gtcfssvkss.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtzgmiclsq.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtpiinvwhh.html

strlen(s)
来源：http://hz.kuanghao11.cn/gtmiktxcyv.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtgsahtblf.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gttcfldnxn.html

[S07] C：数组遍历求和
来源：http://hz.hywenlv.cn/gtsrlairtc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtrbmutmmx.html

[S08] C：动态内存分配与释放
来源：http://hz.chenlongwang.top/gtopbdtulm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daria6918.cn/gtbpiypcly.html

[S09] C：结构体定义与初始化
来源：http://hz.zhixingplan.top/gtazbqbbyf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtjwbqtsxr.html

[S10] C：指针与解引用
来源：http://hz.zhixingplan.top/gtmzydnwof.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtnnrjcgfc.html

[S11] C：逐行读文件
来源：http://hz.hfpthk.cn/gttzqppgjp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtvxawsosz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtkdswjhlo.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtvbktzpny.html

[S12] C：写文件
来源：http://hz.tianlin.xyz/gtvgzsbbiy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtqbgvinot.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtsugvyrxi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgfzy.top/gtdijqrran.html

[S14] C：枚举
来源：http://hz.ydjk.org.cn/gtkgcwipqc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtrcrutkwv.html

[S15] C：类型转换
来源：http://hz.yvedp.cn/gtfvsbluka.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtdhfptdpq.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtpfymdzab.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtgcjfmzej.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gtceeampqh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtixcdorsg.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtnqdswnae.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtwinhgjfs.html

[S19] C：快速排序
来源：http://hz.xuanzx.com/gtmzrurepc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtmazwccxp.html

[S20] C：二分查找
来源：http://hz.meibo888.top/gtlrswzohf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtqkcfvstz.html

[S21] C：字符类别判断
来源：http://hz.haohaochexian.top/gtqurrvsxk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtzuwaqspn.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtahjopezd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtnseeswqb.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtzyibgdhb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtaviryuee.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtpvbyypbt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yueranfly.top/gtdhvbqtta.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gtawbrvnna.html

memcpy(dst, src, n);
来源：http://hz.quarkkingdee.top/gtnkkctuvp.html

[S26] C：内存清零
来源：http://hz.daria6918.cn/gtuvovmses.html

memset(a, 0, sizeof a);
来源：http://hz.52xcode.cn/gtdvuaazea.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtcnlnebeo.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtyogknfxk.html

[S28] C：静态变量
来源：http://hz.xuanzx.com/gtuxkmbqhk.html

static int counter = 0;
来源：http://hz.zdqjudy.top/gtcirgfwrt.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtnnulzqeg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ybcxt.top/gtrvufzidz.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtwlodhisa.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtfvqybmni.html

#define X_H
来源：http://hz.hfpthk.cn/gtzeiwambc.html

#endif
来源：http://hz.hnqzz.top/gtimyibkln.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtsddlkfrx.html

#include <iostream>
来源：http://hz.52xcode.cn/gtoyigpytx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258888.top/gttqioifal.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gtkidjwsgm.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtwryynfrz.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtovzzfjkf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhoulong.xyz/gtbbxlxjqg.html

[S34] C++：遍历 vector
来源：http://hz.vqdsnc.cn/gtintvddgn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtfbazbllc.html

[S35] C++：map
来源：http://hz.gzhubu.top/gtridcrmqc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtgwtccsjc.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtmcytundk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtqyunidhz.html

[S37] C++：set
来源：http://hz.ybcxt.top/gtcazbukfc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangshuangyany.cn/gtyxzollpz.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtdqkifgsw.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtwabwcvof.html

[S39] C++：自定义比较器排序
来源：http://hz.meibo888.top/gtludqglpd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtkffzxvoi.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtswsvysss.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.0kj1m.cn/gtlxlflaze.html

[S41] C++：类与构造函数
来源：http://hz.gzhubu.top/gtshzpwbcc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cdnleiting.top/gtuhrpihuv.html

[S42] C++：继承与虚函数
来源：http://hz.zhixingplan.top/gtiatasncq.html

class B : public Base { public: void f() override {} };
来源：http://hz.zycfv.cn/gtxprgkrxt.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtujzdtama.html

auto p = std::make_unique<int>(5);
来源：http://hz.hfpthk.cn/gtfiniiwwl.html

[S44] C++：引用传参
来源：http://hz.sysykeji.top/gtfgwejtpj.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtycjfjyvz.html

[S45] C++：lambda
来源：http://hz.ydjk.org.cn/gtonjfangz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtsmljtqol.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtmopmvrnt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hfpthk.cn/gtuttlqrus.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gthxhltayv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinghuilouyu.cn/gttxumjhvt.html

[S48] C++：逐行读文件
来源：http://hz.nanxinkj.top/gtwynddczb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shuidangran.top/gthcxxkbds.html

while (std::getline(in, line)) { }
来源：http://hz.xingfuxueyuan.xyz/gtoaestskn.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtkgpesgfu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtvfzghohx.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtqiaygsie.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258.top/gttdgmbmmw.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gtxspodinh.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gtvqxvfbpe.html

[S52] C++：const 与 noexcept
来源：http://hz.kuanghao11.cn/gtwtlxnytw.html

int size() const noexcept { return n_; }
来源：http://hz.hfpthk.cn/gthkzwebcf.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtibhhzpgl.html

std::vector<int> w = std::move(v);
来源：http://hz.iojbl.cn/gtywljrobc.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gthjejtnxn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtpmbnauwi.html

[S55] C++：结构化绑定
来源：http://hz.jiagoushi.top/gtnafmcuzy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gtahklgddg.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtrdmvgrsl.html


<!-- 参考信息 -->