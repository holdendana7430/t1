代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.sweek.top/gtitdyzzuo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtfnewwqne.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtdfuylndi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nwbrower.top/gtxbjwabuj.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtpvljgafz.html

SELECT TRIM(name) FROM users;
来源：http://hz.guannengcc.top/gtyxtgxsct.html

[Q85] 数值取整
来源：http://hz.yj202588.top/gtvvboynvh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.bjfxy.top/gtdamyucqh.html

[Q86] 读取 JSON 字段
来源：http://hz.ybcxt.top/gtjywawnzl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ppjwa.cn/gtcseicgdx.html

[Q87] JSON 字段做条件
来源：http://hz.jianghu66.top/gtnmdvxdnh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtmulfpxbx.html

[Q88] 行转列（条件聚合）
来源：http://hz.zdqjudy.top/gteyrxtkxf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cucudq.cn/gtjwozzend.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aibaodan.cn/gtphmvneds.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtcvbdrpae.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydzc1.top/gtguklajln.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtpkjcwmww.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtovygmnoj.html

================================================================================
来源：http://hz.yueranfly.top/gtrgynrokh.html

R. Bash 专题
来源：http://hz.cucudq.cn/gtiosojgrd.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfigpmqka.html

[R01] shebang 与严格模式
来源：http://hz.chenjidiqi.icu/gtuxtvvbvf.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtpchykhrg.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtpzkgtbga.html

[R02] 变量赋值与使用
来源：http://hz.jinghuilouyu.cn/gtmzlntpvu.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtysajnghw.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtjpfsihgs.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtavsshovs.html

[R04] 位置参数
来源：http://hz.jinghuilouyu.cn/gtcecxrzrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtxtyohhir.html

[R05] 参数默认值
来源：http://hz.smart0.xyz/gtfuaijcox.html

name="${1:-default}"
来源：http://hz.shuidangran.top/gtrlyskxom.html

[R06] 判断命令是否存在
来源：http://hz.zhiwuduotai.top/gtunjukzvw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtnvglhdfi.html

[R07] if 判断文件
来源：http://hz.yueranfly.top/gtnyyhzamh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenzaomai.com/gtgaentdfz.html

[R08] 数值比较
来源：http://hz.fzhhl.top/gtmyrpahxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258888.top/gtnirpbngt.html

[R09] 字符串比较
来源：http://hz.jinqigfzy.top/gtopkhifbg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtkbkxdevw.html

[R10] 正则匹配
来源：http://hz.cashguo.top/gtqqryxrqv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtvekzgmuc.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtjuausrrd.html

case "$1" in
来源：http://hz.guowangkeji.top/gtqcclhcis.html

start) echo "启动" ;;
来源：http://hz.xziqi.cn/gtbyfnkfzz.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtevzkdnnj.html

*)     echo "未知命令" ;;
来源：http://hz.cucudq.cn/gtoqevyxdk.html

esac
来源：http://hz.ppjwa.cn/gtasjeizwb.html

[R12] for 遍历文件
来源：http://hz.sxryk.cn/gttdjgitfx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangshuangyany.cn/gtrisdhhup.html

[R13] for 计数循环
来源：http://hz.52xcode.cn/gtqnrdlpfx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtrixxufyr.html

[R14] C 风格 for
来源：http://hz.chenjidiqi.icu/gtasknhvss.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gthmtvaxlk.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtfxnqrtvf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtqqzvtoob.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtqvyaehur.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fzhhl.top/gtijtwfmko.html

[R17] 数组定义与取值
来源：http://hz.pycfn.com/gtwkhmmpzb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtyqxawmmk.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtkogxecos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.0kj1m.cn/gtpkulwprd.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtzzutjfxv.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtnrucatip.html

[R20] 关联数组（字典）
来源：http://hz.andypj.xyz/gtwfxkusgd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtidcnqmhm.html

[R21] 字符串长度
来源：http://hz.guowangkeji.top/gtyyswbsmb.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gthhrpzbnm.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtxdssowvu.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtdjxtyqqp.html

[R23] 字符串替换
来源：http://hz.chenjidiqi.icu/gtjuxfsysh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gogol.net.cn/gtnhsmabuz.html

[R24] 大小写转换
来源：http://hz.haohaochexian.top/gtvlxzylwc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtikpbnhjy.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtvplslbyi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtjixolkfj.html

[R26] 命令替换
来源：http://hz.wangshuangyany.cn/gtqejfsaot.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gtwiqiluas.html

[R27] 算术展开
来源：http://hz.zdqjudy.top/gtdxxnpfcm.html

echo $((1 + 2 * 3))
来源：http://hz.andypj.xyz/gtlcyqrwvi.html

[R28] 浮点运算
来源：http://hz.sxryk.cn/gthneaqlxr.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gtbuhorsme.html

[R29] 定义函数
来源：http://hz.yj20258.top/gtahkrarrf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtjsdqfmlf.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangtech.top/gtwqhkskat.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtdlglysfw.html

[R31] 局部变量
来源：http://hz.kuanghao11.cn/gtyvaikbvw.html

f() { local x=1; echo "$x"; }
来源：http://hz.ybcxt.top/gtaxlcdnou.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtefvggtyv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj202588.top/gtcjfnmnby.html

[R33] 捕获错误并提示行号
来源：http://hz.dashuyun.cn/gtnamtwtng.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtzuhbkngr.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtuoypwlye.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtzymvsepg.html

[R35] 后台执行并等待
来源：http://hz.jqgufenzy.top/gtopycqrtg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cqqwz.cn/gtdmqdxdyz.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gtdhvoqwda.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtjrmjmxgl.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtamdcjfhf.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gtamcmklie.html

[R38] 管道串联
来源：http://hz.xingfuxueyuan.xyz/gtqswkusnh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jianghu66.top/gtgairyhjh.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtjcktjjpf.html

cmd > out.log 2>&1
来源：http://hz.iojbl.cn/gtjosbrogl.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtssllacqp.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gticysncuc.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtmjvqgafc.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtzprkthom.html

[R42] 输入重定向
来源：http://hz.yueranfly.top/gtitngrsna.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtwqxoejio.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gttzeifthw.html

find . -name "*.log" -type f
来源：http://hz.xinyue.icu/gtzvrcsfev.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gtsxusdpdr.html

find . -mtime -7 -type f
来源：http://hz.tianlin.xyz/gtxnmhxofy.html

[R45] 批量删除
来源：http://hz.hfpthk.cn/gtdqcseecb.html

find . -name "*.tmp" -delete
来源：http://hz.bjfxy.top/gtciqimscp.html

[R46] 递归替换文件内容
来源：http://hz.xuetiantiany.cn/gtremjhlcb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.snrcjt.cn/gtkbtbvdlf.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gteamzctsu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gthhvrvrjb.html

[R48] awk 取指定列
来源：http://hz.dashuyun.cn/gtmlycbudr.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtopgnmmov.html

[R49] awk 带条件
来源：http://hz.cashguo.top/gtfkobgexy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtruiyeiea.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gtrruicxph.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shangyingyoupin.top/gtthdtdtkj.html

[R51] 排序去重取前几
来源：http://hz.yanxiufei.cn/gtjvierslt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hammf.cn/gtccmwlpkx.html

[R52] 统计行数
来源：http://hz.yangfankeji.com/gtppveigrt.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtwzyeusbh.html

[R53] 查看文件头与实时尾
来源：http://hz.c1oappe.top/gtgmcnsnzm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxuanxn.top/gtcelzcjkp.html

[R54] 比较两个文件
来源：http://hz.chenjidiqi.icu/gteegsglnv.html

diff a.txt b.txt
来源：http://hz.yuxming.cn/gtfszzjfen.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtxlrwamnq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtexywoeph.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtqgtzzkps.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtlcjfxoey.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtonhlqywp.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gtywfcxwzi.html

[R58] 下载文件
来源：http://hz.jlsjyb.cn/gtkqkbhwon.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtfemecfsb.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtfyhrennq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtyeimlcql.html

[R60] 只看 HTTP 状态码
来源：http://hz.smart0.xyz/gttlzpfqpp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtyagxvnqs.html

[R61] 磁盘占用
来源：http://hz.xinyue.icu/gtuemdujwg.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtgfdvkrim.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtzvhfxpaq.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtuieulfmi.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gteohtogrh.html

free -h;  ps aux | grep nginx
来源：http://hz.andypj.xyz/gtdrjfflxc.html

[R64] 结束进程
来源：http://hz.gotoacloud.top/gtcpqtvjbn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.0kj1m.cn/gtwfyzmrii.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtdsghoicx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtowzeyreo.html

[R66] 定时任务
来源：http://hz.cdnleiting.top/gtnzbcrglz.html

crontab -e;  crontab -l
来源：http://hz.jinqigfzy.top/gtdflbudco.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gtotsoqtwq.html

openssl rand -hex 16
来源：http://hz.yuxming.cn/gtswwipdrq.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gttfawnutu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtpclhqpgp.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtjytpyzps.html

head -c 16 /dev/urandom | base64
来源：http://hz.gotoacloud.top/gtqhmxvvmw.html

[R70] 时间戳与互转
来源：http://hz.hongshengwenyu.top/gteytgtqsn.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtbzzhivyi.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtwtbtvbxp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtoecqzlhk.html

[R72] 等待端口就绪
来源：http://hz.yuxming.cn/gtytbmegyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtmusjehse.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gttljmbfwa.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtmhpbbckn.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtulgxhgcp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgfzy.top/gtheafvrnw.html

[R75] 导出环境变量
来源：http://hz.sxryk.cn/gtxvorqdnb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gtkdjhuuex.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtjrcglbrp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtbpmfkurn.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtcvxyrcne.html

read -rp "请输入: " ans
来源：http://hz.nwbrower.top/gtcayezfsj.html

[R78] 交互式菜单
来源：http://hz.svipenyu.cn/gtdtywjass.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtqacuatpx.html

[R79] 解析命令行选项
来源：http://hz.daria6918.cn/gtsaglkxzq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangdashe.top/gtghmoopjx.html

[R80] 查看脚本执行耗时
来源：http://hz.guowangkeji.top/gtubzerkwl.html

time ./run.sh
来源：http://hz.kuanghao11.cn/gtnkngqcqe.html

================================================================================
来源：http://hz.havefunace.top/gtqvxhjxus.html

S. C / C++ 专题
来源：http://hz.hysaishi.cn/gtdcktgpqw.html

================================================================================
来源：http://hz.yuanzhike.top/gtuzrgeagn.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtrvweobqx.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtcuoosled.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtnisscydm.html

[S02] C：变量与格式化输出
来源：http://hz.shuidangran.top/gtqmuvjhxr.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj202588.top/gteyczdert.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtdslnhwio.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtisqzdqat.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gttjvufpwh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtalmzgljn.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtchgpxffa.html

strlen(s)
来源：http://hz.xuanzx.com/gtjlwmsnxz.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtiwqudjfk.html

strcmp(a, b) == 0
来源：http://hz.daxiang520.top/gtuwclfkfz.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtlgdkjeag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cdnleiting.top/gtlqmmbvvo.html

[S08] C：动态内存分配与释放
来源：http://hz.cqqwz.cn/gtzyemtnws.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtcwfmzimq.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtogodmelk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtrfamkubc.html

[S10] C：指针与解引用
来源：http://hz.fzhhl.top/gtgnxniain.html

int *p = &a;  *p = 5;
来源：http://hz.jqgfzy.top/gtlkyjpnbt.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtorzhrjrx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gtcnjqwgus.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangshuangyany.cn/gtqdbnjaas.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtkpedwndh.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtlwpehiqn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtpiutwkkt.html

[S13] C：宏定义
来源：http://hz.dianchejie.cn/gtykgcsazs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgfzy.top/gthvzpepud.html

[S14] C：枚举
来源：http://hz.aibaodan.cn/gtrhouuflr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtyhnsprwi.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtqmvrbgxj.html

(double) a / b
来源：http://hz.wangdashe.top/gtitjflwkj.html

[S16] C：位操作置位
来源：http://hz.ydzc1.top/gtoyvphhzg.html

x |= (1 << 3);
来源：http://hz.cucudq.cn/gtlhmxxmoe.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigufen.top/gtrrwnizwz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtgluyuzpm.html

[S18] C：命令行参数
来源：http://hz.gotoacloud.top/gtuxetcbop.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gthjagqkih.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtzcwuxwoa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtwaehryjl.html

[S20] C：二分查找
来源：http://hz.chenzaomai.com/gtaarjuovt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gteyxjsesw.html

[S21] C：字符类别判断
来源：http://hz.nanxuanxn.top/gtqqhznegm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jiagoushi.top/gtukdyctck.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gtjozsvkda.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hfpthk.cn/gtkvivvwuv.html

[S23] C：随机数
来源：http://hz.yanxiufei.cn/gtigdpmafg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtstqqeltm.html

[S24] C：获取本地时间
来源：http://hz.bjfxy.top/gtcytadayz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pengpengdd.cyou/gtuesmmvoh.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtogevmymh.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gtupbprthe.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtnbxxutpb.html

memset(a, 0, sizeof a);
来源：http://hz.hongshengwenyu.top/gtxfqjnipj.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtxwrgxqmm.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtfxqjxsru.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtaqwajvev.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gtfpommous.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtptjzsgmy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtbovgymze.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtuprrknpx.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtbbsfrdyb.html

#define X_H
来源：http://hz.ydzc1.top/gttvizsaio.html

#endif
来源：http://hz.iojbl.cn/gtbzjeuhpc.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtocmzjqaq.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtvvnstcvi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gtgruyzxoe.html

[S32] C++：字符串
来源：http://hz.shuidangran.top/gtfpxrszeo.html

std::string s = "hi";  s += "!";
来源：http://hz.wangshuangyany.cn/gtumlbmlhs.html

[S33] C++：vector 增删
来源：http://hz.jqgfzy.top/gtmuwxfyjm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtpicpanrd.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtvmcjfwpm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtklkonarr.html

[S35] C++：map
来源：http://hz.guowangkeji.top/gtnuumuwyc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtoflxcvzb.html

[S36] C++：unordered_map
来源：http://hz.guowangkeji.top/gtqphlwcgx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtyhdazqkt.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtsmtoqchz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtqbzxcshy.html

[S38] C++：排序
来源：http://hz.haohaochexian.top/gtzcutmewl.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtpakfcfdv.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtbuuniooy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtyecmuxcb.html

[S40] C++：查找元素
来源：http://hz.pengpengdd.cyou/gtorbmmjkj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ybcxt.top/gtvopeddeh.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtxmngcabt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtpyyjsaeq.html

[S42] C++：继承与虚函数
来源：http://hz.c1oappe.top/gtnustwodj.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gturajhdvx.html

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gtontzzbxf.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtgbdkyhnd.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gtazxpttrd.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtwcufchoy.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtrfxrgyxc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fzhhl.top/gtcrxzfffx.html

[S46] C++：函数模板
来源：http://hz.ehwqpu.com/gtuvwdenjf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sweek.top/gtfezofwrc.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gttjmxygyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zdqjudy.top/gtnzxvckvb.html

[S48] C++：逐行读文件
来源：http://hz.xziqi.cn/gtctwzfjdy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnqzz.top/gtuiptdlkj.html

while (std::getline(in, line)) { }
来源：http://hz.aibaodan.cn/gtpglojmkp.html

[S49] C++：写文件
来源：http://hz.cashguo.top/gtluzxciel.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ybcxt.top/gthleiypzg.html

[S50] C++：格式化数字
来源：http://hz.daria6918.cn/gtkktnnaug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtfywzwuup.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gthsnqvwxe.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gtjhxvhvrj.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtwpxzoogt.html


<!-- 参考信息 -->