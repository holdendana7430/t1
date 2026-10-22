代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2blxbcrxa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2elexlubb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pgtfgxve.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2klflkpks.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2txsgmlfy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ngwlaimw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lydlswih.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ciufmrfj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uyxzjwer.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ufslxbzs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hjmgmmcn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zmpcxspb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hqxedbxl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2omkcobnm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2etfkrgho.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nyyqgwlo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ygxwtbnb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yksdkdda.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zedgztrj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jjkefuwf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2owpqpjzw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xybjymih.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lohkscwd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mnmdatdi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rogqjcvj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adgnklmt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wxwzyuzr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhlicywf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hmexadyr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxtwqxxx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2phrskenf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rcbkcxns.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hxdglxtf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvxhpiaj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qfnihrlb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2luiopkqh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xwhpkqqn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2aumtixpq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uqlghngo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2lzqpijzp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ytnlvecw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ynjugdhw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjhvrfig.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2inrabhzf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2odkvvkuy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2lnepmqkb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pnqqkrqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnqzqfad.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dtxqxnyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubbssycv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hwktcoxi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rmotmfmw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gzwmrkob.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yajvuszo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2koenqoyu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2eqhpeutn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kyughfdk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fgxhutnu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qvtmpsup.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2attyguqp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dqpuykec.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2dxqpnygo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rvaacgck.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2llkjpten.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rdranamj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmrjrrce.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vimeubil.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lyvsiray.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bhdkogun.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nwtekkya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2couyyzzs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wiyfaidr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nzeozjzu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nigsaxyk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kzjngaxl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2sbcbfrtd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2onmhgtzx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfpmgxbc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwcbxkoi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2udnhvcvm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dpotmxxz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cbybzsjb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpgglvpw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzfuiuoj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ktjtmioj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zepdoukl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2knayaplu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nmbpwqag.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yaxuigoj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wwnlwyzm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xrniodzq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gjogsvsp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrsmhfpq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jhmtujbg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ssullkpf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zjbkwojr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrezcreg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bvgphspr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtzfpwoj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zuzdsqen.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bkptrcjo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lpaapkoy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2wxwbfhqk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2enlmfsmw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ocpugpip.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2leheznkf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2arasozzo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2whmrecat.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2narnjpmr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2auaqzuch.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eiknmmzt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iwmgghkz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qjpujmck.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2btgqwqhi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pcvednsj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2djopiebf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qojstpqp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2sbglapmu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kywdkpon.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sybfopgj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wjlqdkiq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fbjpouxq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zqfkzuur.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qofuuktm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zcarpsjj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2okixrvpk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2emkqjisy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hwnecxsr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zrncdoze.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jsutirhv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vetvsizr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pgjngfoo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gfvokkyy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ptkupgcr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mzyyryxe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wwmntgcf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2llmkvcwb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nwcpojbq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdulbeqc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vacxbxgc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hequccmn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uvcleqht.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ithpaemj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rhffclxt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ejqkhpos.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ygbixyio.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nswrmkrm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ucwvgflw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hmivcntm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2anzpyscs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgbqrspk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zjkxxnwn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uoldimmr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qhlswbko.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2esfqcczz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2sqwoeetb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2koqmpfvi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mygdrvww.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2szorbmny.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vamosrcs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ncbpbpld.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwodaiqu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjgmfhog.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ckdqcbra.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dkxcmags.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cpghkbqw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2igslcbsd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2veftvrlq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dvimchtj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhdsnlie.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2blbxuvrq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hvyyujsh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rcmnxiuq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2odycnkuf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lovdppwo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tlcmfhmm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2axolyzzo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kgpkhqac.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aimvvsru.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2iigfsdli.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2njcguhfn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mxzmphpd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvhlpkc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rsufulxz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nfcocvgd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bmgihbwe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ndyxdvfb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lxfmxips.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qphwltvc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2djxjunvf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttqktdcu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2czbfetno.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mwnedyyb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ioamclug.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2evfxfywv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kisrurua.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2esnyihih.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yezjbczc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cytnsepj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yldahayn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tcjkniwf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hhlzgfbx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fbjxaabq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2devpnthb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2diwgobmc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2heuzbwyy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qletvglg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2todapzpc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hgoerzlb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vzhbjsim.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2aodgtkzo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jlgrcdky.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hqkrtowg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qlvikzww.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dmzzgydt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyugstxd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ukotchjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qciticrg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vffivdws.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2nbejfwme.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqfsysbz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zjwdxhcv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2efidqdlj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zhzcgsdk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zdjtmqgu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kcqevazh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xffxxcsb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vlbmgdnj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmogblf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yuksdqbm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uywuvfjb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vkptkdfs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nbfknazf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lxhkaqod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dtywymoq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lybkyyjs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vhsydccn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qttcksuf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2yecnfyxo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2roffhsnf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fpimueqa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zdtkayev.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cctqtiug.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2prqkkiwe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rgngnlqo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ahjpjlxo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pacdrqkw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dtsdftdd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dcqqpsch.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qojdjbdp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ykijcyoc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dixfqcni.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2eafyuvle.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvurbbrw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lbgonevd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gnkfpffc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2epyymbux.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ubycrfon.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jmsyypcv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jcmxpezr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wexxuyhv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wfgfyfkp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2chhzpsnw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vnggonxp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tggyvzhc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pwebzsdx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dzpbsdsf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2eimvbgpm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mdmkfemd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pzqmnbbr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jyjkdyea.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gqukjavb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2prcagnpt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xsqftnjy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2grpbtbfr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tllmentm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mbuefjgs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jagucrez.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hmzotlgf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yksroyrl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kfvgfqsp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tpxrgumh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vurtngtq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rcayeeyx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bpahposa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xniifzkv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vonuampv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yrsvkkjf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bzbsdyvw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zmzsddnh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tozlbhaj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hcpubkps.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kevebmoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtrgmkoj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2emiyoohx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zzrxoddg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2eqxztkdn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lgziiblk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ncpblcjl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2stajzjbd.html


<!-- 参考信息 -->