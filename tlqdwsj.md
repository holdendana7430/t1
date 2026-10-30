代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gkafgcunv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmaxwiuwa.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsbzsihi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggarhmupz.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gesbmeigd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gocmkjhcv.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gzheqmqzi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gcmawcreh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwxxhoko.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcubqjmyz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmqazpyh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbaiosxf.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/grkylpwnh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gilqxfpdj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guzdfvuat.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpktfjoql.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gaegepagz.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyoaoqtv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giowuvevo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gupyfuhqj.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubgwwzcg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gixgvpdxc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsubcstl.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/grjbwxbip.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxyrcpka.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgwloigd.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gscriduvn.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gezsfcjvu.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gjpnuwboq.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/grzcsuhop.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gqknibenz.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiaanywj.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlzgttim.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gfscnnacs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gskvavxch.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhlhrcn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/guoxysbyu.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobdwoar.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/geoiiegtk.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gesgchjjg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcvnjepu.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvbzdvug.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjxlyesas.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gimmeqcnp.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gkklxfsgi.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthuudqaw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gldnwtngx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuinijda.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gximxlkfm.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geatioknc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gznathfge.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/glptmwxad.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxirqofms.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gwauxtsex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwnebwvk.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtslrgfgt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gihdajapj.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/grurxgmvb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoloctzv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaypkxxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnjnkyrh.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmuavuzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwdklpx.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrtpxrxb.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gendokqzc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxrkbijt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdoxgjno.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggiqnctzy.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrzoudma.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaezojua.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzzmaxbps.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gokwzcldn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghelkmguo.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gacuspggr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbehjwpod.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrxvsaax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxntfrez.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gengvezay.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdaeaxcn.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gaxzecyde.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gnmmdskoe.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvjdgbtd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvlsovvl.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwevejey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjezufpdm.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwgqrgzb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoirxxmo.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gadwbfylc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkrrsjgi.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gelhkpkts.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtesggspw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gxsekinno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gbaakyrsu.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gxuylxxpn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ggkxvenxp.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gvifmujeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelezhurv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnauqgfb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gyioeytnj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiugbgib.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxspdbll.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gsvojtzhy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gakwbnqeb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gsdqcnqmf.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gytlhyliv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gaometdmi.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gbjdhdwyx.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzazfyoeu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzalojzx.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqtwkqrd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnveerrf.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdxaztts.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gznxiqmts.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfipmikly.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/guiiioagx.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnekcyyp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gwraphorq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzvwnrmp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbygfqhd.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gawtbsoeq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqzigbkpb.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxupihgt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmawptxzl.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtxtckam.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gzsmkymsa.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gxymvyvlg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdoqhbhe.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/garvskhqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gnlfeyofr.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwgklimu.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkedomkm.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gthjnoojz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gyuhyxqoj.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gghufeeeg.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glvdwdtie.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gnvxstafs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gecseivpm.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gphrsgwgb.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmchnpak.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gqevfqmct.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzomvkxys.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxndqdddo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gcpdzkxiv.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ghfvqokem.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqytppnf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqpgvzyi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gyopfifct.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwdglda.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvgvrslj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghpyzdkjf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gldlhuyib.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhzjdnvd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gikfwnxkr.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrwbetus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtrqqlrx.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknpgtuao.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gpuhpuzrg.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gtcxhboji.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaiekmxq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gemenkorp.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/guubmfgaf.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gipmteavo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghekcyeqe.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghecbezrf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gveucvrkj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfwcnppf.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/grswkbmjn.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/goyiilzya.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdcpcure.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/ghwnulmuf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggmjwmmcy.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnwrzzgm.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gpqrgtufz.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gnrpscuyg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guylfnyuf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxurzsamx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrvwtufg.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjcrztfag.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grrutpruz.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/grkmlllqe.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/guypnphfo.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytppoxyz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqvarbkz.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gqpqnwdrs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gonfhavon.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gbohtnroo.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeewukrv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtswawwap.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlnwvhsa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grndgdbcd.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grqlghrqe.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/grenbdott.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gangncywb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gizhpvwng.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuaiudgy.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqqilkvo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjkdycym.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucmjeevs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvblnpxlx.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjzdhmoqa.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtaagldz.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gywscrgex.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzufjkdhw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnlkcbwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyaruwyc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gjloohldi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbijqkop.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/guyqiqegv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gjochahhc.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhzzwptx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gkwejfujj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjfjwegkz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupdrvave.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garnvpbpi.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhvsamdq.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gncobahnk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfruryph.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gegqsayjo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwokbyybe.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/genspikau.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkviaquln.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gauclyfqy.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gxpjolual.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gzgbeekwf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvrngqvf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfmzikoa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/guptaxhzf.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxtclhjwd.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/guxdljdoh.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gyuhylrwv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdimuriur.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxflznhx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gejsydlrv.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdihkjdc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmqjjldl.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gozaiaxvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gbpdrhiej.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/geerrmddd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gpydysmli.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gebkumaty.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdpwlbyi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gakjcqses.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywrrenxh.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gbtostvbc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/geitqrpxy.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjhtife.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjcdnixj.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glbubebnp.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxzcrgv.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmidnstdn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtslhnnlt.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/grxfwdckz.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzwjfezdw.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpcwykze.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/ginxfljyh.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmachbglg.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/grvrtekyc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfldnbedn.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfmiqbet.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiggwdao.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/ghfjldrzd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkniigntc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjisifyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/grkpoorja.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gklylxjsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gykyhbbbh.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gplyzzode.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhglzlan.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjksefzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcivqpab.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjmspeha.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gglergujx.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjlbspbz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gllpgkezi.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gorlsubed.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqfderny.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnlgnvlta.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhlvnlgv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggzihxqzi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvivhzb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greoorqqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gokrxiwtp.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/grwanhgwo.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqimoslqd.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/geojrocha.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwgbzaeh.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnjebqus.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnqsdiisu.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhimhahh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwolvipkm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutrtfotx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gyjvorwbc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gegskklgn.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/glemngebu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gyfptnkwr.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxbrsqop.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gevqszqfr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/geogarkks.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeltemok.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gimoihwtn.sHtML


<!-- 参考信息 -->