代发 wailian999

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnlokjgfx.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/grqehwmnd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gweiuvlsx.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gbxcmsxpi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gggtjgprm.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gnkbjfgao.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gneqmnqea.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gmgjtxewx.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfysbqigu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gnovpsexo.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gpglvorrm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gyxblhjuk.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gcfqdvbqf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gfdeciewf.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gvwwqfhyk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gduovbegr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gtbglogob.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtnpdsfzo.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gunnkjjow.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwfudrxdl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gfwrayvvu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjhoglztb.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/guccpeuak.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfaaejrqs.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gjappuned.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqshkogog.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gtclymrfp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gfhwxxauj.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gbpfairex.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gmiboquwi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gpkikdnuz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gvudfcvkg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gsqtlyhhd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gjogngiko.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdrubwcgm.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gffvnojoo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gorvneldn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gdtxftsmj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/geseygjji.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gugxpnmtc.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gibphxvis.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqxzucqvh.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gupxamapa.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gnvoebysl.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gvvbypzfa.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gletveium.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/giqthmqlk.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gzkpsmbhy.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gkyfliuxr.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gdvohipaj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gseyrkwft.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gbzkkgurm.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gmpjwsuyf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/ghzlefxgv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvacsdc.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gbsfciaxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/grwablzji.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gptxeztui.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/guanpgelo.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gmgywusay.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggacxbqns.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxlwwolxu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gkxrrhedl.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gutbwmcoa.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkfhxgk.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gwjapmuiy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gkvyeewoz.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkuddgcgc.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gtthfbmly.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gmkpqtzzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gzdsaqrgc.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gpvmugywg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gewnnydsz.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gvzgodbqo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gfxptiimw.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcsojzpel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gflblujms.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/grfxufihe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gcqmbnvuw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gfdgorcpk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghejmgbvq.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gmrrfbjcx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/giqonpbiz.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gcsrecyzg.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gncjkaytj.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gwzrdbodn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gwqwrsdyk.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gdnphzybb.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gsolmpjvd.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gezundebk.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gccmbzxtd.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/goqplcbrl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/ggfvmkvox.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/grcfufzpk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gyvinfnsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gahynyeom.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gemxygzfa.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gaboukvkb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gymvryviu.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gtkspdrbu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gbmzbaiqw.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gqfgevxhl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gkzkndgdj.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gftbjvnmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/goutuwkhs.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gfzhwstqh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gmfvxynlx.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gsuhxsdfl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gtcjsctqm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gjxbtjvfg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/goeygobqg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gutpkvxdy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gmdyosvob.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gsqihdrzv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gnwbesqys.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gczdsbtjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gzgixzhom.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gzjulhtpy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/guxsxnaln.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gxpzuriwi.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gpmznwhun.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gtgtcsihi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gyxtoouqp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gweidnrgv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ggwvtiehn.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gwnvtmxxf.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gygrcoakw.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/grlnzjhfj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gguccolhy.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/goagdrgmf.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/ghiayirpk.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gfbnyqivv.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/goiajmmio.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gjxgoshtp.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gfvtyftcz.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gahajiguq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gamwkplhv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gfpcttolb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/grvuspzgy.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gvqhqiyun.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gfutdelpo.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gxvwobrxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gearqmdql.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gfsojrftz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gqmreyftm.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gxbnsxfrm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggzjrgkig.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/ghegsttnt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gegdiwtri.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gxjpiqztq.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/goejmstcf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gperlsqwe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gtgzqsosk.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gbiwkpshm.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/glmmrkhva.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gzzlfvwsc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gwcwoshag.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/ghynzuegv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gxzbeozyb.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/glfsgbcbe.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gpndunxyw.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/glsftgopv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gyldhyvpa.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gzlihqrau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gizgpepeh.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggtojdfgj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/glzzjyzyv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gyqcvhhxf.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gcydfosax.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gbmhfjoho.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/glalllhem.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gmehtvqyv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gnnnbszsz.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gyibeoeih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gtpqaellh.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gbhksbswz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gzyavlyuz.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gznkegikx.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gwokdrrsx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gcdhczskw.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gzvceejay.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gzpfbevcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/guvokiphi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gftuhqeaw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/govwjkuxm.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gsjviavux.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gdncolrpb.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/grccvvduh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gdjiliygf.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gpulwyqcz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gcnaqobxo.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gnbhhoxbg.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gpbrzuaam.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gpgftqrfi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/geybqaqoj.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/grlysjofh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gpwzsmczs.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gruqnqums.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ginrynskq.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gredtltoa.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gkraumrar.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gkpvwbktd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gvfdjilbc.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gbqvlcfsr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/goyzvkief.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gnepqbllb.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gnptqogcq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gamuekaae.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gmycqsaxb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjgecnqaz.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gomkrksbl.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gbthiusam.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghnvswlke.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gdbxqebvx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/geoeisyvd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gqzyljwnq.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gxdxvgyro.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gmlzzbmsb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/glziizxsr.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqaqnubgg.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gnoefhatc.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gzdxltfiu.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gbwueogej.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gnvwqvqwo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqvlaei.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gpkzqvgir.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gndphrjze.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gbiubvhhh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gwadtoqwq.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gzixzgtet.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/guernprgj.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxwmnsbzc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdqbtepar.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/guvrxwcoy.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gysoybvvt.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gskecaiwl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gizfgegsw.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gdwwlkfmx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gpyxrprep.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/galdnosin.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/glgskflxi.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gfzkhxgqs.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gvzvzfcsq.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gfvcyizes.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjytrjbr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/givigznik.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gomfrqjry.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gnefgvasi.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gzhflmmmz.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gvvxfmvox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzboeigfb.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gxphlonln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gybimxwuq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gpmilkmbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gnsntrybq.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gnvjkpcfm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ghwggvwny.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/giiajzfqb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gzxtheony.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gtxggxwjh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gqxemashw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gocfgpvvz.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gzgispsax.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gujhlzqnd.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gkrocmzus.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gjjctwslo.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gurpuamqi.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gytbmhefr.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gwtrocelf.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/glsjaabyq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gknqurros.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/ggnboniux.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gvzwhpvir.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gzukhkocr.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gexamzzfo.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkztsyzcy.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gllsswuyu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gbozuwrsc.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gsuiofoag.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gunuddxyp.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/guetdgyge.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/geqgeauld.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gyhjoomvk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gxyweitcw.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gswnshvzv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwdrujxpj.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/grfzebfib.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvkqtpxiq.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gknigyzfz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/geoppqysa.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/goqvdfoyg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gxekaqsyk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/geldnaboc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gbkspqvev.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/ggddmzabl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/ggputkwjs.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqgpgkifi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/ggbgxntja.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gjbtoxzyv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gebynochq.sHtML


<!-- 参考信息 -->