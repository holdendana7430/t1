代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hbwunjmx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2feawvgnt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2cyyatpfj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mrexqfgf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uveggfht.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pczcseqj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tfszgjmo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bvshhryz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lestjuks.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2porlzbcs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nopmwqyq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wdftnzuj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fzykhgbs.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hrayjtlw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ndgrfxzz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2lpsilbev.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qxslirco.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bmeyjfuf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nfgzutqq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zfgmznkq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qlbsbrcg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bnaxkltn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vsxbgflj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kqfqsjms.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2azilqjhd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hocjmdvh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2todmxpbv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wasxdsvd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ylxdircj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkijrbtr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xcyfdopb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iypkqaym.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2heayweug.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2antnitrb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2sieugkix.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2slwurcbz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2funraxao.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gycsevjh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zllmbzqz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2sopdmobg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kkqohdmy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zjunttnm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljdnmusj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mnslwbop.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wbrkpgbj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rohcjmkk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2npjzzdze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvuprkqm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ehismucy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vldcztts.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ccxyhrbh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wlpcqzyh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pnpgpnbv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ehkzjljz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2icilmmru.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tvpmybtk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qfgfymzr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2lxivzulg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ghxvucjj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cvbjgwco.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ptqqblrs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nvfknvui.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwkvtved.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ivrzhiwe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yypuvcma.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jsomedne.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mawpzsns.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ewinkiql.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2lmybexli.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rfnchevj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ohmsesuz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2byhuaogb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2npwfmzwv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2srgppanx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vvnfxcpa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2raqnnikp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2quukljos.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nadvcyrk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tcfunsxb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yllgnqtj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kvmgdwgw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kpdlhtun.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kwzygxrc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqobuwlc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2drstaplu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qlpghntj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ksftrofj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hbgtsach.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zybztstq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2shmrbrri.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rkguemqy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iakbgnyj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wjnkfzli.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ukrhinuq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sbwnsgdm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dsvpfwvm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2enasllts.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nicpzsdn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2gitflwxc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vubwtljd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2amzahyse.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jycjtyrf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ibubugju.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qpdggdet.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uftnhoeq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bhzhiypo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2arlfiqzs.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rrzbydxt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qhlwknjn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mtkwyjjt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2izhyldlj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iynhguim.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ggzqbbrl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2owzrmsun.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kzqtpcyr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2leihqzcm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xlaucixi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ekortnrv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2idlxtctx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rcfgcmir.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2oxozmcux.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jnhzeeky.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lkqgcpyp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2znoypwia.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2orlfadqu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qeogtvdp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tscevkae.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ldjeqpdn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wuuqmaqr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uhtzymop.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2oyysbyvl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ajdudxch.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yinxeyte.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lheonnas.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2czdzjsju.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2epytmixd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ykqgzmeb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bkkzplic.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qtsuwelu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vptsgjow.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hugfwqgw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2duklbwbx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yjtvzarn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2idnlqmhr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bzbtwowv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nmvkghwd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nzgfgbll.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tmwnrukv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oyvmkgng.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2htjihwja.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hwqaoxnb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vxienzoh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nuuwbccd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qnecufla.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qukpipht.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cnysfqmi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2njisnnoh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nggkqflf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2osfxuwsa.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ndurmaee.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gpbjuwmc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gtqthigc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qzwkfeiq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nrbwbbie.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jfokavms.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hlektbny.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bebpczmn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2llbpquqd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xbqxjehq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bowklcyo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2lkxokokz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zmlmmgbx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tjtbdoyd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2smbvtnrn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2oeuxueje.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2rqylckib.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ofysmvop.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwscrcmv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2texahghk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sutextsp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2elbklejy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2szcdaliy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2coivytha.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2eyynifhb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2twvvtntx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ujamqlxx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lklogmpk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jffjooga.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2awcbcwhu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fondocxk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2csahtiaz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qizvpkwk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pqplqcpk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vsquyexg.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fzrdnskz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jgktokso.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jzcbpxsn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zeylrtin.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipztcmly.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kdiynfkr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sfoqzjqw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2quitybyj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2myfbbbkp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdglnuwv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2aposeznk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yxdelvna.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2urymvtub.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uqrefdzf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yeubrkid.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lkhcbrlk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxjocrvb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uffuugjz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpxixzux.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wqrjaurr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dbzggvkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcgjckco.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jolscvxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nscwbzsg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jmsivesz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fwcuzjql.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lieplecu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2avbyfuym.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bkzrzbxz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nwyqxtap.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sduiphug.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2knzyuqnv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bewrhjxd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rqdrgxou.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcneyse.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jkutavvo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ugpqonhz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xmexeino.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tcgcufwt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2plvomzym.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sxrabgmn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bwbwjnfq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zxoypfmp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2texcljbb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ibyrryzn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qamybiou.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2djfluair.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qxiktjhi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rohvrcmk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jspufvsv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nmyraylf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aubxbjqs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rxxaotcx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2khguffds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rhdmoito.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dllpqmqt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zgqkjkzj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jpulvmst.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gwxbftne.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqsiloea.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fnjbdbqt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2stdcxyar.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hygmezwf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gyjffoks.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gqesokgx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oerpsdpn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jslugzpk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nqhvlsih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rpmydqyw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2toqnkkpv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2osgfhdbp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ccwleinz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hucrcfnc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2sgbjtalb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gnpsjiii.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2thvatuma.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yztsrjea.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ylsrpwsv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cdntieiv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lbofcsff.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yeblunje.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lyviqnop.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2riqwfrjd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2azvtbfxi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2acymzdxz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wgeubunn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bdeltdrf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ikbsuwqg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2axxhqlgs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zzzdsquj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bkbkaufu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jzywqhys.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pfpoppir.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hrixpclo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2umjyxcen.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pjusgkum.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jugdpmgg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tidzsnnp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2yactvvqk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mrzzwalf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dogzugwg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ysqruuwb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qffnaqlo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ubytqdia.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2braykazn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tweryykv.html


<!-- 参考信息 -->