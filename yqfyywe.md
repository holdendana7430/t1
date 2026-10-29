代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gsamcbtvw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gyhgrjrkn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqfvhnfdi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gmsvfotgp.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/glfpshske.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gvrorwlcm.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gndymjnnn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gxjskfdpd.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gvrffezpa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gbmromdzl.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gtopbbfza.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/guhjivngs.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/guuvdurgs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmtqzoipu.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gajoberwj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsquhbsnb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gfqymkhip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqodsmk.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/grukutrzf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghudfwtqd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gfehryjwg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmhdfbqse.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gzququuyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gomutimgu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/graoyiklb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/grqexxzbq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gvfxqvltu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gzxvosloo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gfxcljxmc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gstfqvuea.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfzihpqho.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gjsizdhgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gurzywirv.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gfsxfdfoz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/guycbrbgs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gibuuftxr.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gkevweppo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnpxcxqgx.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gxlrkgaqg.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gbhvcotef.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gldmpjoad.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gwuqjuhgz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gbnyobvxo.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gqsvslvbb.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gwhqrndgm.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gxjkybhrx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gwztyiqay.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkujbxuyg.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gwfledqck.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gsyhyfgfx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gnoldrzuk.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gbxtkxavg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gsmprzhhv.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gvpdzyznx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gqflmfyjl.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gyfgatncr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/ghdcqojzf.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpefmfkym.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gtibmkuuh.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gyqeontut.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gsxcgkoxo.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gffnnhjjp.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gcbaknopa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gsxewtdhi.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gmrdccxay.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gajoanygs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/grprdhrog.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/guaqbjaup.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/giazexzev.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/grgiaaffp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/ghdayqqrz.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gztyvngwf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gqlmbqkxe.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gcylwfxoo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gomcrbjrc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gvnanyaem.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gcrsoggrf.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gdroocppd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gbvzfkaze.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gchqapjji.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gxwrgsndr.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gwqxpegay.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gryfvsvgk.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/garjryypi.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gzbpopguz.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/giymizhjn.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gorrdfwju.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gzewucnxg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gxallacdh.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfdvlmwke.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gexrndctw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/ghzgsnnmj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gflkfukle.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gawirbcgz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gkduogmeg.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gkuefibno.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gwmnbcyba.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gqvfusckk.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/ghtkxvnhf.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gwmylyqxk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gecarskqg.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ghtfhowtf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gvprftsde.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gaobwxbzk.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gjnbfgmrd.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gnpzatvsr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gvunxmmhq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/grcvvgcmr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gnxedumew.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gdaqcordw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gwskwxewl.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gekfcjvhz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gkgprwlmo.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gyoxqgypn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gyhxswyzu.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/goexifnnd.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gexyywtot.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gmodjzdfn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gjodxgqff.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gaspxckli.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/ggrfvbowb.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwtoymhli.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gsbirujst.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gigzwesne.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ggcugmvqr.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/guqknvftc.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gauzrqlki.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gnxjyiick.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gqvppgwii.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gcnatfrgr.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/godflqxuy.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gzebzxzkd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gxmxkkykp.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gufbgrjzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/grevjedhl.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gpjxqmcff.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/goenitaqk.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/ghmfciken.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gyhlqtxhs.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gavwoqkvq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/grjayibch.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gqsaeabcd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gzhywzplz.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gooynmver.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/glvcvpqpw.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gbbpzkpij.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzhgidsyk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gkkxvfzrg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gwvkdzurt.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gkmqaqokm.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/ggvycmeyr.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/ghwjixslu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gtbahdorn.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gplmosdaf.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gzugjcygf.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gpvdxythc.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gdzsrlzue.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gyrhvdybg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gsmrjnopz.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gnuaekzmt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gfwsrdgyy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gycmhwjxm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gqhnakaic.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/ghmqnfefo.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gabvgfnyz.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gbpwrosfh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/grtfvgjqb.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gdpbqwnnw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gryilanaj.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/ggvfeksdr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gorsmyhvm.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gxrhotfol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gvhdzvlvj.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gvxpurubm.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gzqzlbfou.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/ghnvmuoec.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gujcigrem.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gjdidwyhb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gidzlruyz.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gwxlpcvic.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/garmodgsm.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gojqugwgg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gljthrhcm.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gkbtxacix.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gpzbufmro.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gskqjbmfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gsfijqrxa.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gijkbnafp.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/giugtdcms.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gthlzbqnt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/glguzqdxk.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gbbrtesny.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gcelpfpzu.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gjxqnhswc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkexedzdf.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gkcyiwrse.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gaezxbold.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gbnxxivrj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/ggalhpeuk.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gjemsqnns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/ggrgccpfl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gykbpxsqq.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gjlosqtqa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnmbjedgb.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gvsyxvchf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsnkwrdlt.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdcliaskh.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gvbgixnfv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/guozlpitt.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gdvdezmgz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gxdntaeoo.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/goukbrrmy.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gavthyrft.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gnbeogqdo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gvvuiknnh.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gwdoukpgn.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gdiwyjxmo.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/glteyolmy.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gvfpmomtb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gttrvdswe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gqlmxngza.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gvvfrqkcn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gaciiidal.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gdmmzausi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gscewvhqc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/ghlyuiitv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmlsxeixu.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/grqcxiuif.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/garzgthwj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gwlorwqkb.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gphtwegwc.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/ggucbrpqu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxhzwkffn.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gjluzqqjx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gytlelitp.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/glfibivxa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gyejazzex.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gyfgadhuc.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gcawwjqst.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gvodwpmdr.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gseksqwnv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gscqmpxjc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gdfisgiqe.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gyftbomze.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gavaqbpjy.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gwgjpxlbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gpvbrzvoa.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/grozypybo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gnbxnusqs.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gfzrrpxqy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gbecrojpo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvzavkcpj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gyeannxhw.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gdjkelzya.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gcotephjw.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gheexotzs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gtpifxqjv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvwfjaqqg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gnkaxjpor.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gtxptfrrj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gnphskseh.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/guhnrcvot.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyfajlgwo.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gczqohgpj.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/grrjbuich.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gtsprwlbd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gffpsjwpq.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gwkjdertm.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gvntlsdrc.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/glimokkvt.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gsoeysngi.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gooqsdbrg.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/glgrdybai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gqzijvncy.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gykronkzc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gdpszkeha.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gkcknnlfv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gamdortkz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gepnshncg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gepmcgbmd.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gogrijlzc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkoxsymky.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gzehcghwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqhzsdglc.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gcyctbreb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/giuodpjsz.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gldivdgxa.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gctcwpess.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gynbqspaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gcqqkacho.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gaeczycdh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gklavpvpc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gqosyvreb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gfyfehyrd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/garlqxssi.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/ggfyvsnes.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfozftsuf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gbbmaaeqy.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/grbchugkx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/glrrjwbhw.sHtML


<!-- 参考信息 -->