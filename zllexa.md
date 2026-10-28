代发 wailian999

[Q78] 当前时间
来源：http://hz.nanxinkj.top/gtabrgyixe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gtxwgykqxd.html

[Q79] 字符串拼接
来源：http://hz.yangfankeji.com/gtpjmcinab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guannengcc.top/gtkvghwlkj.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtbkzkqymk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.0kj1m.cn/gtaevnaefq.html

[Q81] 字符串替换
来源：http://hz.sxryk.cn/gtgntbtkax.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtuetinqlb.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtnaybbknn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yanxiufei.cn/gtpalplden.html

[Q83] 大小写转换
来源：http://hz.cdnleiting.top/gtqcksvgda.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gtetkbkgoe.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtmlursrrc.html

SELECT TRIM(name) FROM users;
来源：http://hz.jianghu66.top/gtwxgdimkm.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtxnaazqxh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daria6918.cn/gtzplfusqe.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtcsrprpdv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guowangkeji.top/gtofxcejyp.html

[Q87] JSON 字段做条件
来源：http://hz.chenzaomai.com/gtzhxknfkb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yvedp.cn/gtwrkmdged.html

[Q88] 行转列（条件聚合）
来源：http://hz.aizwys.cn/gtkdwkukxp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangkeji.top/gtcpwqxpkh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigufen.top/gtmxjngrbu.html

[Q89] 判断表是否存在
来源：http://hz.yuxming.cn/gtizxgagwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhaomingkeji.xyz/gtlducklpc.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtriktvlmj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtrucfiipq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtybqmnpse.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtwubavhni.html

================================================================================
来源：http://hz.jqgfzy.top/gtewsizrxw.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtdvzdedkg.html

#!/usr/bin/env bash
来源：http://hz.ppjwa.cn/gtkpmbuwol.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gtvpoaolkd.html

[R02] 变量赋值与使用
来源：http://hz.havefunace.top/gtzhlngszq.html

name="Tom"; echo "$name"
来源：http://hz.nanxuanxn.top/gtltwvnzzy.html

[R03] 只读变量
来源：http://hz.gaohongyu789.top/gtzbozqhjo.html

readonly PI=3.14
来源：http://hz.daria6918.cn/gtujgmvaio.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtlfltxddg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cucudq.cn/gtnibomifk.html

[R05] 参数默认值
来源：http://hz.snrcjt.cn/gtydswmsjx.html

name="${1:-default}"
来源：http://hz.cqqwz.cn/gtrgnchjhc.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtkmdybqos.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtczfffgmw.html

[R07] if 判断文件
来源：http://hz.hfpthk.cn/gthufekdla.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtxoelhxla.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gttvvdxegw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yueranfly.top/gtzzkvfkaz.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtrfctfmke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtxyithhkm.html

[R10] 正则匹配
来源：http://hz.xylfe.cn/gtfutjczqb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jiagoushi.top/gtrmlktrsc.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtqcfzogrd.html

case "$1" in
来源：http://hz.fzhhl.top/gtdtbvcgie.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtzzkbxels.html

stop)  echo "停止" ;;
来源：http://hz.sufxvd.cn/gttzhgaapw.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gtvtowbynx.html

esac
来源：http://hz.havefunace.top/gtbingsxaj.html

[R12] for 遍历文件
来源：http://hz.9152youxi.cn/gtapoczbph.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guannengcc.top/gtoyuecqll.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtmljeglxb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtwvazfvgu.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtjavflhnr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gogol.net.cn/gtqznnhnop.html

[R15] while 逐行读文件
来源：http://hz.316326.xyz/gtngeafgqr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cqqwz.cn/gtjhocfdlv.html

[R16] until 等待条件
来源：http://hz.gaohongyu789.top/gtvnvdrbvp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtekhljrgf.html

[R17] 数组定义与取值
来源：http://hz.daria6918.cn/gtxfiavjdm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuxming.cn/gtxrlvodlk.html

[R18] 遍历数组
来源：http://hz.zhoulong.xyz/gtngajlukc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuanzhike.top/gttihfxcug.html

[R19] 数组长度
来源：http://hz.havefunace.top/gtgxlrswwx.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gtckfxswbn.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtxnjzzeat.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtphtuatak.html

[R21] 字符串长度
来源：http://hz.zycfv.cn/gtovlqvdpv.html

echo "${#s}"
来源：http://hz.shanyushiyangkeji.top/gtwrndtiln.html

[R22] 截取子串
来源：http://hz.cashguo.top/gtalwalqfq.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtmsbuloph.html

[R23] 字符串替换
来源：http://hz.zycfv.cn/gtrzxepchf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtojsqysfi.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtcxyinrjg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtfspqaxdt.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigufen.top/gtvxtwjqaz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtyxwnnbwu.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gteuseysnt.html

now=$(date +%F); echo "$now"
来源：http://hz.9152youxi.cn/gtmnrkdvnn.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtowsemrfa.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtpzdjwxop.html

[R28] 浮点运算
来源：http://hz.sysykeji.top/gtshlchkzb.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtkhecxchp.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtfahfiygc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangdashe.top/gtbxjdecng.html

[R30] 函数返回状态码
来源：http://hz.xuetiantiany.cn/gtuvobrzgj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinqigufen.top/gtilrifiag.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtqulxpsih.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtrzhrjgcs.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gtcvxccbwo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daria6918.cn/gtkwvwhcmm.html

[R33] 捕获错误并提示行号
来源：http://hz.yuanzhike.top/gtoqfudrms.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtuzjnozqj.html

[R34] 退出时清理
来源：http://hz.yongpay.top/gttuzgfiec.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtzlzapgno.html

[R35] 后台执行并等待
来源：http://hz.daxiang520.top/gtkvaksrhy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gotoacloud.top/gtcwyisqma.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gttffqckzz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.c1oappe.top/gtpheuyzht.html

[R37] 把输出赋给变量
来源：http://hz.jinyuanbaomall.cn/gtklaydrhz.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtuwfldnmc.html

[R38] 管道串联
来源：http://hz.tanke756.top/gttmyyaibf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ehwqpu.com/gtkitfqrbx.html

[R39] 重定向标准输出与错误
来源：http://hz.cashguo.top/gtctzjoubu.html

cmd > out.log 2>&1
来源：http://hz.nwbrower.top/gtdcxfblsz.html

[R40] 追加写日志
来源：http://hz.hnxiangtu.top/gtungarpch.html

echo "log" >> out.log
来源：http://hz.yanxiufei.cn/gtbznzdlvm.html

[R41] 丢弃输出
来源：http://hz.yuanzhike.top/gtgbhujpth.html

cmd >/dev/null 2>&1
来源：http://hz.feifeiyinyue.top/gtivarcowm.html

[R42] 输入重定向
来源：http://hz.havefunace.top/gtiodjejln.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtydzjiism.html

[R43] 按名字查找文件
来源：http://hz.yuanzhike.top/gtyrjxoshi.html

find . -name "*.log" -type f
来源：http://hz.daria6918.cn/gtxwrjwxvm.html

[R44] 按修改时间查找
来源：http://hz.zhoulong.xyz/gtzmohwpzt.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtfpxvwakz.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtbkmwzkpp.html

find . -name "*.tmp" -delete
来源：http://hz.ywan-chungtsiang.top/gtniysmedf.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtgulrjpgr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhengqikj.top/gtxqagcvgk.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtxpgilerp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gogol.net.cn/gtoszmzpvv.html

[R48] awk 取指定列
来源：http://hz.jinqigfzy.top/gtcjnrxxhb.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtozaqrpum.html

[R49] awk 带条件
来源：http://hz.hfpthk.cn/gtpztojbcz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtbaxmbdal.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtamimclkm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gtrkexkbou.html

[R51] 排序去重取前几
来源：http://hz.ybcxt.top/gtjusteouo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dianchejie.cn/gtedgcaeup.html

[R52] 统计行数
来源：http://hz.sufxvd.cn/gtqrwotyft.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtrwtkkzqp.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtxtgzesaz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtiqteldax.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtjuidaqkm.html

diff a.txt b.txt
来源：http://hz.fzhhl.top/gtkvmtxqff.html

[R55] 压缩与解压
来源：http://hz.sysykeji.top/gtikdrisst.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtvkscaumf.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtnytdeowb.html

scp file user@host:/path/
来源：http://hz.zhiwuduotai.top/gtxzuzrqad.html

[R57] 远程执行命令
来源：http://hz.andypj.xyz/gtxsasmeio.html

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtmppurbse.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtledtovpc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtfygwqoxt.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtliivalqm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fengsongda.top/gtbxymkzir.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gtsapmbkqa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sxryk.cn/gtrvvmighq.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtjslrewpa.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtgxbbcjsd.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtjjzqfpqz.html

du -ah . | sort -rh | head -10
来源：http://hz.kuanghao11.cn/gtzmkxwbqt.html

[R63] 内存与进程
来源：http://hz.gotoacloud.top/gtxdnzzuyy.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtjqtdcxjl.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtpjtlcwfm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.havefunace.top/gthbrzliix.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtskrpqorr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cdnleiting.top/gtxddwojci.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtdtnlsfph.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gtacyktixp.html

[R67] 生成随机十六进制串
来源：http://hz.jqgfzy.top/gttpttkxtb.html

openssl rand -hex 16
来源：http://hz.xingfuxueyuan.xyz/gtrkrzvlxd.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtqgswmbou.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtvwsuzzmx.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gtogbqpzkp.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenlongwang.top/gtyqkaqswd.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gtlcesukag.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gtdgaiytry.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtcclsvwyu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtjolwhxvn.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtnrrljhwg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtihdehncb.html

[R73] 分割大日志
来源：http://hz.wangdashe.top/gthgkrzpwv.html

split -l 1000 big.log part_
来源：http://hz.hfpthk.cn/gttqeggyqw.html

[R74] 批量重命名
来源：http://hz.vqdsnc.cn/gtsgilfqip.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangshuangyany.cn/gtigwqxocx.html

[R75] 导出环境变量
来源：http://hz.cqqwz.cn/gteikbkqkq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gtnzhifqey.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtmxzlfucp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtuzhhlmee.html

[R77] 读取用户输入
来源：http://hz.yuanzhike.top/gtydnxyhpj.html

read -rp "请输入: " ans
来源：http://hz.pycfn.com/gtlcijanay.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtzgofcviy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtlrvkcril.html

[R79] 解析命令行选项
来源：http://hz.ydjk.org.cn/gtandowklg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj20258.top/gtqegtzsqh.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gtgmcabjbm.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtpcsmwwft.html

================================================================================
来源：http://hz.smart0.xyz/gtglpbartb.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtdljsnjci.html

================================================================================
来源：http://hz.jianghu66.top/gtihybhxhh.html

[S01] C：Hello World
来源：http://hz.shangyingyoupin.top/gtxsxklcmk.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtjuyrqyds.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtsdmwabba.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtjhiszhce.html

int a = 10; printf("%d\n", a);
来源：http://hz.zycfv.cn/gtbopitoze.html

[S03] C：读入整数
来源：http://hz.52xcode.cn/gthgjjwnxd.html

int x; scanf("%d", &x);
来源：http://hz.hfpthk.cn/gtudjzxqlp.html

[S04] C：字符串复制
来源：http://hz.jqgfzy.top/gtdbpjqqbk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtynlidhbw.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtgihgenir.html

strlen(s)
来源：http://hz.snrcjt.cn/gtjkorpgsh.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gtgincjrhz.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gtcpjbryav.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtdjjnhymq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jiagoushi.top/gtjfexwulz.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtyfjbykok.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gttfmvlejo.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gthzehials.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtglbuwwpc.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtbedklzci.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtqntncygr.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtasqtdoyi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xziqi.cn/gtodcwhuzw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.bjfxy.top/gtiuevnyfa.html

fclose(f);
来源：http://hz.xuanzx.com/gtbmizwrlv.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gttfoteqik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gtovebiokc.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtxvqkxlmy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gtuppmvkls.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtnypbkfbi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangdashe.top/gtybddrvdp.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtlzvgcewa.html

(double) a / b
来源：http://hz.jinqigufen.top/gtpqcekewx.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtybzwzsfo.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtbvbvxopl.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtxjgkjndb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtjutjacpf.html

[S18] C：命令行参数
来源：http://hz.316326.xyz/gtpengzmjx.html

int main(int argc, char **argv)
来源：http://hz.xuanzx.com/gtdrczezpa.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtmlpxbtgq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtnfqvytjz.html

[S20] C：二分查找
来源：http://hz.chenjidiqi.icu/gtqzoqumnw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtahvffucb.html

[S21] C：字符类别判断
来源：http://hz.zhengqikj.top/gthlbpaqvy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtwgkxegua.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gtgvikvtra.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtsjzuxuup.html

[S23] C：随机数
来源：http://hz.tianlin.xyz/gtvrgrdoft.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gtxtvnhhyw.html

[S24] C：获取本地时间
来源：http://hz.guowangkeji.top/gtfgsqnagn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhijiandao.cn/gtblkqmvor.html

[S25] C：内存拷贝
来源：http://hz.jinghuilouyu.cn/gtehlbdppz.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtrfyllyaw.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtuxiaclkm.html

memset(a, 0, sizeof a);
来源：http://hz.guowangkeji.top/gtreomapwq.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtgdbdwemy.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtioeecxzp.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtnyccmjbv.html

static int counter = 0;
来源：http://hz.sweek.top/gtibldktew.html

[S29] C：变参函数
来源：http://hz.daxiang520.top/gtnweztjwc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gtefgbvfus.html

[S30] C：头文件保护
来源：http://hz.dianchejie.cn/gtvnfycarc.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gthxvoeoub.html

#define X_H
来源：http://hz.jqgufenzy.top/gthbikjsuj.html

#endif
来源：http://hz.xuetiantiany.cn/gtzyudgiwc.html

[S31] C++：Hello World
来源：http://hz.zhaomingkeji.xyz/gtklwxvmqc.html

#include <iostream>
来源：http://hz.hywenlv.cn/gtdqnehqgh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtrbuppjal.html

[S32] C++：字符串
来源：http://hz.snrcjt.cn/gtvvywphin.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtbryggqbk.html

[S33] C++：vector 增删
来源：http://hz.hammf.cn/gtzklihjwc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtqrvppuub.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtgbrqqmre.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yongpay.top/gtbrbqfpih.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtshtjhzhb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gthsazfcxc.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtfxejapih.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtnqqoaqxt.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtsnuxsuov.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnqzz.top/gtjgjonmgz.html

[S38] C++：排序
来源：http://hz.zhiwuduotai.top/gtosermwxd.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtcsafopvk.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtgfvpdcii.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jlsjyb.cn/gtdpukvzhe.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gttspjmioj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtlxectzzx.html

[S41] C++：类与构造函数
来源：http://hz.0kj1m.cn/gtforltikw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtjmfrgszr.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gttiwslhtc.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhiwuduotai.top/gtrsqmrmeq.html

[S43] C++：智能指针
来源：http://hz.birdmap.top/gthrbrwsme.html

auto p = std::make_unique<int>(5);
来源：http://hz.cashguo.top/gtmyffjjyw.html

[S44] C++：引用传参
来源：http://hz.chenzaomai.com/gtnuniixec.html

void inc(int &x) { ++x; }
来源：http://hz.jinghuilouyu.cn/gtilhdoapn.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtkjppjbdt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ywan-chungtsiang.top/gtrokmucbi.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gthrvfmfjg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtxenmkgxt.html

[S47] C++：结构化绑定遍历
来源：http://hz.dianchejie.cn/gtqtbvhzwg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xingfuxueyuan.xyz/gtultbwcxc.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtijfrprki.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gtzddcfcdj.html


<!-- 参考信息 -->