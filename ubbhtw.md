代发 wailian999

ANALYZE TABLE users;
来源：http://hz.shanyushiyangtech.top/gtbsxbsnyx.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtgpxzwoqy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhoulong.xyz/gtsdxzbsjm.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtfwgicmad.html

SHOW INDEX FROM users;
来源：http://hz.shzxlz.cn/gtjanauzsg.html

[Q73] 查看表状态
来源：http://hz.tian-w.cn/gtsxymcjrg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtcfwwbtzr.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtzhdzaqqk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinyuanbaomall.cn/gtznfijqqp.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtwyxyivof.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhiwuduotai.top/gtnpwonqsj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xinyue.icu/gtfaarrhgx.html

[Q76] 按天统计
来源：http://hz.pycfn.com/gtcblzeyvb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.redwolf501.top/gtncubywpo.html

[Q77] 时间加减
来源：http://hz.gzhubu.top/gtwtznlngu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.vqdsnc.cn/gtmfdmjawb.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gttpbbjqvo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zdqjudy.top/gtgtwgaedi.html

[Q79] 字符串拼接
来源：http://hz.tanke756.top/gtxpasacgp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtfiewnfxh.html

[Q80] 字符串截取
来源：http://hz.wangdashe.top/gthtbrgczu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtfjymitkm.html

[Q81] 字符串替换
来源：http://hz.tianlin.xyz/gtostgkdqd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cqqwz.cn/gtfglfzupo.html

[Q82] 字符长度与字节长度
来源：http://hz.jinyuanbaomall.cn/gturoctsvc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.kuanghao11.cn/gtbdgrnxgw.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtlphorlfl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gteaudcfts.html

[Q84] 去除首尾空格
来源：http://hz.jinqigfzy.top/gtcztsodve.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangdashe.top/gtopdskovr.html

[Q85] 数值取整
来源：http://hz.chenjidiqi.icu/gthvxhdfgo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.9152youxi.cn/gtwdybkosy.html

[Q86] 读取 JSON 字段
来源：http://hz.zhijiandao.cn/gtdcwhqziz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtwqfoznlj.html

[Q87] JSON 字段做条件
来源：http://hz.0kj1m.cn/gtysuoiqcq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhengqikj.top/gtnkhefyzg.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtyzfixafl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtkucqqasg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtfmdbaifc.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtndbvnnag.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jiagoushi.top/gtthsglvew.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtpzzmykln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yanxiufei.cn/gtfjmftpol.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmuyleyzj.html

R. Bash 专题
来源：http://hz.mhx1999.top/gtjeqwoith.html

================================================================================
来源：http://hz.yueranfly.top/gtgtbpudym.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtmpaxtkxa.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtkoxxhldu.html

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtsvatleyd.html

[R02] 变量赋值与使用
来源：http://hz.0kj1m.cn/gtmjmyqtcg.html

name="Tom"; echo "$name"
来源：http://hz.fengsongda.top/gtkyurcmrs.html

[R03] 只读变量
来源：http://hz.yj202588.top/gtlfovusvf.html

readonly PI=3.14
来源：http://hz.yueranfly.top/gtovkjdenl.html

[R04] 位置参数
来源：http://hz.9152youxi.cn/gtfukchjkr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigufen.top/gtjiqteuiw.html

[R05] 参数默认值
来源：http://hz.andypj.xyz/gthweecsgp.html

name="${1:-default}"
来源：http://hz.yuanzhike.top/gtfjzadkzm.html

[R06] 判断命令是否存在
来源：http://hz.tanke756.top/gtgbdkjkxe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtcejhzzhh.html

[R07] if 判断文件
来源：http://hz.ivvv.top/gttjydnqen.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ivvv.top/gthkvcgxcl.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtsieqjbyh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtzckmbzfa.html

[R09] 字符串比较
来源：http://hz.svipenyu.cn/gtqjkluozu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtnvzhknzv.html

[R10] 正则匹配
来源：http://hz.xziqi.cn/gtfbsqmolg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtytlwqigf.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gthsbushwo.html

case "$1" in
来源：http://hz.gaohongyu789.top/gtipgmunox.html

start) echo "启动" ;;
来源：http://hz.mhx1999.top/gtrbfyqzkp.html

stop)  echo "停止" ;;
来源：http://hz.shzxlz.cn/gtqeyvcboi.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gtppuzwmie.html

esac
来源：http://hz.bjfxy.top/gtkzvdencw.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gttmvmxell.html

for f in *.txt; do echo "$f"; done
来源：http://hz.9152youxi.cn/gtfyfotwtr.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gtndbqobua.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtxrjezicp.html

[R14] C 风格 for
来源：http://hz.birdmap.top/gtijlgglna.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ehwqpu.com/gtofykaulg.html

[R15] while 逐行读文件
来源：http://hz.shuidangran.top/gtyxxmdmdf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.meibo888.top/gtpntbbhbs.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gteetittmc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gtnufyglvb.html

[R17] 数组定义与取值
来源：http://hz.cdnleiting.top/gtwfkyjfgg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ybcxt.top/gtazdmbazm.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtedqwsdyp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.redwolf501.top/gtalgngjtf.html

[R19] 数组长度
来源：http://hz.yj20258.top/gtbezoalzs.html

echo "${#arr[@]}"
来源：http://hz.gogol.net.cn/gtgjrxqlgk.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtttjzncxz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtcabbtlwa.html

[R21] 字符串长度
来源：http://hz.wangdashe.top/gtslqqlbxy.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtgdspajpc.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gtopfthxxp.html

echo "${s:0:5}"
来源：http://hz.bjfxy.top/gttiufezqe.html

[R23] 字符串替换
来源：http://hz.ybcxt.top/gtdvdboqrd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtzetnjshk.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtafxyfqij.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhaomingkeji.xyz/gtyyzvjpks.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtynvotnri.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnqzz.top/gtgjbexgoi.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtjmzzehzu.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gtjwrmkawz.html

[R27] 算术展开
来源：http://hz.havefunace.top/gteudjbsvm.html

echo $((1 + 2 * 3))
来源：http://hz.kuanghao11.cn/gtmxfnyksi.html

[R28] 浮点运算
来源：http://hz.redwolf501.top/gtogankwsk.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtghbzopyg.html

[R29] 定义函数
来源：http://hz.jinqigufen.top/gtbmcziytj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtubeakums.html

[R30] 函数返回状态码
来源：http://hz.pengpengdd.cyou/gtyaecrxvx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhiwuduotai.top/gtvtqewxwo.html

[R31] 局部变量
来源：http://hz.gotoacloud.top/gtptqfmddx.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgufenzy.top/gtbkdxfrcp.html

[R32] 参数个数校验
来源：http://hz.hnqzz.top/gtyocbwdjd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.52xcode.cn/gtsvrztpyw.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gtwykeuzhr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gtojrrwepc.html

[R34] 退出时清理
来源：http://hz.kuanghao11.cn/gtjvsdmweu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gthzvbrayy.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtvtdzcqkr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cqqwz.cn/gtxnbestyk.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gthhcofzwd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gtztepfgfl.html

[R37] 把输出赋给变量
来源：http://hz.xingfuxueyuan.xyz/gthlxlghbr.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtxlihrwso.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtcfemjuts.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtjlcusqjl.html

[R39] 重定向标准输出与错误
来源：http://hz.redwolf501.top/gtgjfmssxj.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtacbaoflt.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtydutfpsr.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gtdlsjuvwr.html

[R41] 丢弃输出
来源：http://hz.pycfn.com/gtfiwsntsj.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtnaeogqex.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtsqlfaxme.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtclaqnivk.html

[R43] 按名字查找文件
来源：http://hz.nanxuanxn.top/gtobxgdcls.html

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gtnwkdqenm.html

[R44] 按修改时间查找
来源：http://hz.xingfuxueyuan.xyz/gtnjddoupj.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtbyuiuhlb.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtcuniicim.html

find . -name "*.tmp" -delete
来源：http://hz.hnxiangtu.top/gtfsicfyre.html

[R46] 递归替换文件内容
来源：http://hz.xuetiantiany.cn/gtgfsoqqls.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daria6918.cn/gtcehhxbwl.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gtnyxsmgrc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtgsdtgmad.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtisllxufi.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtbknmxfxm.html

[R49] awk 带条件
来源：http://hz.zhiwuduotai.top/gtnwmtwwep.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtnkxggpew.html

[R50] awk 求和
来源：http://hz.tianlin.xyz/gtfqscebgd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daxiang520.top/gtybuflohu.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtyhbaysbs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gtasmnudgu.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtluhbnjzv.html

wc -l a.txt
来源：http://hz.xuetiantiany.cn/gtgbpywlyd.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtejrpdctl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gthozznbhl.html

[R54] 比较两个文件
来源：http://hz.nanxuanxn.top/gtiwvofrlc.html

diff a.txt b.txt
来源：http://hz.sufxvd.cn/gtarouhwbe.html

[R55] 压缩与解压
来源：http://hz.jianghu66.top/gtxqxmarol.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtwykmvyvl.html

[R56] 远程拷贝
来源：http://hz.xziqi.cn/gtwxuqscnw.html

scp file user@host:/path/
来源：http://hz.cdnleiting.top/gtdwcliqqb.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtbyqmrmfl.html

ssh user@host 'uptime'
来源：http://hz.jlsjyb.cn/gtisrekwtx.html

[R58] 下载文件
来源：http://hz.sufxvd.cn/gtbsfwrepn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtpiozjkqg.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtlweeiiqb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258888.top/gtlbfsdhmr.html

[R60] 只看 HTTP 状态码
来源：http://hz.daxiang520.top/gtgizhazat.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtiwekvfip.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtokgvovcz.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtsgfjmfyl.html

[R62] 找最占空间的文件
来源：http://hz.haohaochexian.top/gtmenjswda.html

du -ah . | sort -rh | head -10
来源：http://hz.yongpay.top/gtqyfhehio.html

[R63] 内存与进程
来源：http://hz.jyoumei.cn/gtysgekbvw.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gteiiunbgb.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtlpzvcgcu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinghuilouyu.cn/gtuhawzhyi.html

[R65] 查看端口占用
来源：http://hz.ydjk.org.cn/gtartwwezw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigfzy.top/gtdrszjamw.html

[R66] 定时任务
来源：http://hz.haohaochexian.top/gtuthttivg.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtxaglebnp.html

[R67] 生成随机十六进制串
来源：http://hz.xziqi.cn/gtcwdauvqd.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtqusfngzk.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtkraiqawa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtkzbmlsjj.html

[R69] 生成随机密码
来源：http://hz.xziqi.cn/gtaxmiqpgb.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtrpfjmfyx.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtszfvtirs.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gtjtfjjjeh.html

[R71] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtbsrndsxj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtwaxcgevv.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtteyzhitv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gtasskclbx.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtxlzsumww.html

split -l 1000 big.log part_
来源：http://hz.haohaochexian.top/gtbwyggdko.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtldylbmwk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangdashe.top/gtprqfualu.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtdslrszvv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtakgbrnkw.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtwlwzwkws.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtbkfbaacz.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtdftltmwt.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtzqgyzzkg.html

[R78] 交互式菜单
来源：http://hz.yonumen.top/gtnzudpylq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.fzhhl.top/gtfmoaejsr.html

[R79] 解析命令行选项
来源：http://hz.yuanzhike.top/gtuhwdkcdq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nwbrower.top/gttqabfjtp.html

[R80] 查看脚本执行耗时
来源：http://hz.0kj1m.cn/gtfpenpiur.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtlpqaxooy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgwnhddoh.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtdhrsuwkm.html

================================================================================
来源：http://hz.xuetiantiany.cn/gteusohuqx.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtbtlqqlot.html

#include <stdio.h>
来源：http://hz.chenlongwang.top/gttdfjcyai.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtujopbroy.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtkzdgtath.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtklyxrfot.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtajhimxgk.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtdzfmnmcn.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtpvfeydzx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtewhtddnx.html

[S05] C：字符串长度
来源：http://hz.jinghuilouyu.cn/gtpleiiwjl.html

strlen(s)
来源：http://hz.svipenyu.cn/gtwxgyoqiz.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtwbtbwhhk.html

strcmp(a, b) == 0
来源：http://hz.yanxiufei.cn/gtcdgndhyh.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gtvvqfupmo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtypymcrpf.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtcvtoqwwq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gthxrlrkyb.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtfxohemjn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hfpthk.cn/gtakamojzt.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtulgmtndo.html

int *p = &a;  *p = 5;
来源：http://hz.dianchejie.cn/gtzwzrirsi.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtsgrlldeo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gtjewvapzz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtbsedwbgx.html

fclose(f);
来源：http://hz.snrcjt.cn/gtxygffqas.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtqaoovkse.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xziqi.cn/gtjycdcyic.html

[S13] C：宏定义
来源：http://hz.pycfn.com/gtzwzpdrbp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aizwys.cn/gttdbnawee.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtcckbimnd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtphsnisjd.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtuqepzjpb.html

(double) a / b
来源：http://hz.ehwqpu.com/gtzfowoqcm.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtxjfhfkql.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtsysoxkow.html

[S17] C：安全拼接字符串
来源：http://hz.yonumen.top/gtzqfvuabc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shuidangran.top/gtcondpaqv.html

[S18] C：命令行参数
来源：http://hz.ybcxt.top/gtajoggpjs.html

int main(int argc, char **argv)
来源：http://hz.gogol.net.cn/gtuocfvojy.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtwogwsnur.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtpcoounan.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtalszqsua.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtglkgwiol.html

[S21] C：字符类别判断
来源：http://hz.jinqigfzy.top/gtgmhqxpvu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtcenpnpot.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtatwqgevd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnxiangtu.top/gtbfduoylp.html

[S23] C：随机数
来源：http://hz.aizwys.cn/gtsiuvtqqh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.birdmap.top/gtqfdstlrh.html

[S24] C：获取本地时间
来源：http://hz.chenjidiqi.icu/gtsitaxook.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhaomingkeji.xyz/gtolslkmge.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtpjmxpahq.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtydhdvmzl.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gtgjudvlhc.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gtblcnkrdq.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtelustgbn.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtjoiingmd.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtvdgbocgl.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtkezanjnk.html

[S29] C：变参函数
来源：http://hz.ydzc1.top/gtcytwximo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtsvbgxmrg.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gthkhpexnb.html

#ifndef X_H
来源：http://hz.feifeiyinyue.top/gtxlvguafk.html

#define X_H
来源：http://hz.svipenyu.cn/gtczzwgkxl.html

#endif
来源：http://hz.nanxuanxn.top/gtmtypiepz.html

[S31] C++：Hello World
来源：http://hz.feifeiyinyue.top/gtkqywvwse.html

#include <iostream>
来源：http://hz.316326.xyz/gtgxcmgoot.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtfpllidnp.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtextqlyma.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtinvatzvr.html

[S33] C++：vector 增删
来源：http://hz.0kj1m.cn/gtgatoogtz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtydaqcqhf.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtmektceka.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.9152youxi.cn/gtdnvxiild.html

[S35] C++：map
来源：http://hz.shuidangran.top/gtrlzqnrhk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtzfruxewb.html

[S36] C++：unordered_map
来源：http://hz.shuidangran.top/gtyubxcity.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtflkvtkri.html

[S37] C++：set
来源：http://hz.cheryme.top/gtkabtgjvy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtgltwspwu.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtqbewmhgg.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtaaiuvnkv.html

[S39] C++：自定义比较器排序
来源：http://hz.meibo888.top/gtiooglfyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtnzymmkgd.html

[S40] C++：查找元素
来源：http://hz.mhx1999.top/gtpupobrxm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tian-w.cn/gtkkgkhqpu.html


<!-- 参考信息 -->