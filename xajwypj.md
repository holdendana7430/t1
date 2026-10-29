代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gmqotkwwt.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gdhlaoiuw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfdszuiyf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gnxeiainh.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gtfnylilh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gllvpnoil.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gjilbsgkg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gjyirwgwp.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gwsgabulk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gpnxfttrl.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/geqdzicbx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gwuctarlr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gaktgfspr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbypwkawx.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gdpdomcgi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpmgxqiic.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gjgpoexau.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwkaadsxd.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gbhsstcso.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzyokqcwb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gfvfjpgly.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjakwixqp.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gagvyaxkb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gratouavb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gupvplbrp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gszzyyfeq.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/galnwjdqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/ggmpcwpti.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gahygzseh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/glzfcocdi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/ghtdqhnfz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbaqmbdnk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzbenicou.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gghgnhefw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/giccnuajg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gygcenocm.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gzalnnboe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkrwhbtwf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/giuddvujd.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/ghcnrljdv.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gvjnqkscy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gbvngaqqr.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/ghujaoiyp.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gpyzrovpe.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gixfbgzku.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gqydtnbji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gzebwfqvd.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gdnrkksdq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gewfwkpgt.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/geijwwvgt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gtzployde.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gwansyipf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gbtcuoqeq.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gbxnejfzt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gbqhyyail.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gkesnrseg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ghrltcccr.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gicbpdgjd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gzyubsiit.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gmazxyzrd.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gyiilnnne.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqycyenzs.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ggotzjdep.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gsddunemp.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gwwdnxlcw.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gtuoawyql.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghkcmkvdy.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gfgbofiur.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbzmozuwt.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gmquhzafj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/guqqkexea.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gzlvyvpvj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gptgxlqyf.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gsmesvenv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvdupkmhr.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gvbkttdcw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/guwhcjutt.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gtbfxatqa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gnituinqr.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqylimezr.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gfwtcdesx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gnbyzvpbd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gjcmjwajn.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gacfieziv.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/getpnhtsb.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gbkvzejaf.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ggaftgcnn.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gljpislim.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gmwuxwcev.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gfcmxtaed.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/guacaymtw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gogvoxkep.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/guzksamrt.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/guflbbsph.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gjcijxhbn.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gawnjemdt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gvakcbiin.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gddqwgkpc.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gtezskyve.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gqkstdmbk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gfyojahgn.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/goxvjpbct.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gjgxxixxu.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gwwsbwwwi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gvgayajci.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gssukhknw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gobaosvfd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/guatldvtc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/ggnbcjqcg.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gdwrhblwl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gxihtnmfl.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/grdsxmleu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gnqflbmjh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gwznacpki.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtdukacia.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gsdmwdlbw.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gdmggjqqh.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/geiebbekg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gkkjnhjde.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gjwfwbcpk.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gnktefolv.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gmnuvopcg.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gnjhvlaiz.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gbrdadpug.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gyhmykvtc.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gvdydufde.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/genoajrht.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gcpsxhqcl.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gzmanrqdj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gdbfvwndq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gvhgtfvhu.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/glyszaalc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gbneefjgw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gxqbukrdm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gollpgfqy.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/guxcrglwx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gslogvodp.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/geydwriqa.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqcuvnxbl.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gdnquvdvp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gfgylcqjc.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gklvxfbjk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxhbwrhjt.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/girozgmif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gifzhstsb.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gcgmrzkbo.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gtoyvdzuh.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/guekmxkfd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gcdcutyqj.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gdqclcqjp.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/ggscbihwx.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gswhznaop.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gowkyoxjj.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gifelsnnh.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/grqkicxvh.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gxuajxxhh.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/golitecrc.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gdriunjgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gbhfprssw.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gstriaewn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvaujyfng.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gffpllous.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/getokqexa.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gtegkvtlc.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gamtvfdor.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gtojxfpcx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gjwfefxor.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gfqwybinp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gpgxaomat.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gdrzwhieo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gkamcxewf.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gbhhvkwkx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/ggdpcutjo.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gfadakmfb.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gwxzeohqg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gzopcjqvo.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gpjlmpcbi.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gsdjkxauu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzthgcgue.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/ggsxmzpvj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gprynevdd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gklcrxqhi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gwmwutpxb.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/girxxfvra.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gkaxznwkq.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gfhljimjw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gepvfeuno.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gtrkvdrwm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/grznnvmva.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/goxfjohyg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gcqxfdvun.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gxceehdvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gwnbzvbce.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/ghmxrfuob.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/grbwtouyv.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gpwlrptgk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/grtyvadjg.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gjvwvzxma.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gqplqmaad.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gflomjxlr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gibaopyft.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gsfeqldua.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gahorocwv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzrnobvjf.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gxvrlxbla.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfudfpmkh.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzdqyqrhp.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gxzacmexr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gmqbafqpt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gsbhsncvx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gtdgevyqc.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gcwmnujej.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gjortyixl.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gmtetdyaq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/guekismsc.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gskyccsyc.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/ggnofgaqa.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gnucodwkw.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gzgkaauik.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gtrsukpxz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gdnshgndz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gzyyiammy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gzkfsiyki.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/grwumgair.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gxkhlwbsn.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gfpewojci.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gzvjxwrzf.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwyvtazaq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/ghtwowmrv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gsxbozibn.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ghjsjaxyy.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gyogxnpnq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gxpxnjegn.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gacrzeoec.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/glgghaatb.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gjocrfxai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gmwhgxala.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gymbhggnk.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gprfpgaqn.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gsaupgvzj.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gmvieqeib.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gtxqziyzv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gimgaoexo.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gwleuzgqy.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/grytnmjrp.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gluarjbza.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gunvyafob.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gfyegaaui.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gforanwmy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gvqmbumoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gnddhtiew.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gcwdfcwkf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/ghxbhokip.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gzgurbrpn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gjoguqgsh.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gvjbnjbqp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ghhugakww.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gysalgtea.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gsuydajsj.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gqgrjyzsz.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gzzpanexa.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gzksrjhrk.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnwsjyzzl.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gtuvhqkrb.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gatbqjhor.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gtxsrogfy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ghucqxfin.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gmnrohjyu.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gtnwkaaiz.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gsjivebhy.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gyruvrrym.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gulanwfnj.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gbovoyvev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/giabacreo.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gxppbwpii.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gagsvepqq.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gzaqgsazr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gclllgnwh.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gtgpderkk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/ghrrxmsti.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gzgmfiaey.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/glvldqxxj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gqamdqxvx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gqtlmkgwz.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gbzhmbgfg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gmladjgew.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gpyszdhqo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkalrvjsj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/ggopdmfwc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gzyptyrti.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gwhsepghy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/geaozgght.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/garsglurl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gpbcwxjqg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gbhtcwovp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gkmljkwle.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gypuhqpip.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gjqtcwdal.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gspetdcqs.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gwsbdxvgz.sHtML


<!-- 参考信息 -->