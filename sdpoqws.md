代发 wailian999

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gbrmfcwvs.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gaoanojkj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/grqnnhcjd.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gjqmadfql.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/grsgdtagg.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gypevkkxy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmmxrcgzs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gguuushrd.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/grgfazgof.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/ggumdscfj.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gtovyqxji.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gjorvjrrm.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gfznfoqqj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gjxbpowlq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gyhmkbixd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gboqelqql.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gyldiukby.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gifflgsee.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gtvhqbxcr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjzltrfdk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfxgzasob.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghykujnbg.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gznlzdyhz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gegqhukbx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gzbssgiqb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grdwwgxwc.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gadaravhp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gqlbwikmf.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gcsckbfvw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/giybgsxry.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gtknuliux.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gqgbzzzpp.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gimqbmilk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/ghdvdvilb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gywehlxxg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsrghofvb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/ghaascvtd.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gdexodzzq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gwilqqlbp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggzozpcxn.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gtnldpbci.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyvikdjoi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gxxfjrrwm.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ggkxhywmb.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/ggniexvvr.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gmsfabxog.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gctwuprqv.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gzqqayaun.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ggfcatzqn.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gttjqtgef.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdwcfzu.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gdapordig.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gjozdaiii.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gixdbjhdq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gcpytsnyb.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gvhxfjlwr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gvcqvfbjj.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gcngxllal.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gusioxouf.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gawpkhpjs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gkwwmkwbd.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gnfudlwpk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxffrsdog.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gqdunxzmy.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gpxjkrbug.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/ghqbijqxr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gdnqrirtt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gugnhredi.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gtewykwgm.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gwfqhomzv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gqaobxkzs.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gwoitqvca.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmeaxzvos.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gavuvkeko.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfighludo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gitjiycud.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/ghaqladyd.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/goczrdarr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gqwlajfmy.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gxbjmsxbo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gflxsjhtw.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gfmyxlkra.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/grkdvmobz.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gbatrtqwq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcggyjmkw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gsydrbpbi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gpsnskfsb.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjjvhqdhd.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/ggritrxev.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/guagirebo.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gczxkqkvx.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gfobcidyw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gnkauyywj.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ghjhshhjn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gpgaffcms.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gmiwpwtrm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gnobfczsp.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/grwhvfyvx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gsavcpzni.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gurgdazbx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gsczjsrik.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ghmcssaea.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/grmuprvui.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gayamuhgm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gtmdxvccc.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gjiwlqqrc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gdjmblnba.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gbwnldprn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gdxsvlwtm.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gamgddeth.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/guekcirnq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gkdxtmwod.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gnriqathr.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gjdqgpxlc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gamwmrkdw.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/ggdcegjul.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gixolbmxf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gjfqjehxc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gxkipdvzy.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gzzspwmoc.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gesrzytpm.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gbhqzripm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gqlzvdbtm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gvthnilrg.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gehiylewg.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gylqonsxf.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/grgfrbtwz.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gnqfcetmg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/glgjaxhyr.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gnlqhbctm.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggifzprxy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gabyldjxs.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/giavrrqul.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gyhslzbqn.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gqohshmdk.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/ggceplcqh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/glknztbwi.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gaoetsveu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/geefjzffu.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gtmeweedr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gmzkbsqrh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gqlojyypc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gvclutrgw.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ggjgxbrwq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/galrkpblo.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gjsaxbskb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwkosznrg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gugvtyksy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/glortsbos.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gppjdvbxf.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/grynxrqkf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gmuhxcasu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gegimjndn.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gtvzvkiih.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gunuhvxsa.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gwwzfpbto.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gwdpiissg.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvjmquskm.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gaezlpqhr.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gkfzvldzo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gfqfmqold.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gbsnrbiis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gzvlgsmpd.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gkilukwaa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gqltmvwna.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gvmdmmurr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gbudunoxk.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gzdebifec.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gstojbckj.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gonmcefbg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gxmlzhygl.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gvvfsainr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/ggtcdhnqk.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gbbtnvlkh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gyxxuxzlk.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gbgyzsptp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/ghkkqtulm.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/ggvtzfqvb.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gzuomypjt.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gdygnwmup.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/grpvjgohe.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gbujctgiy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gjuqderht.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gzhlmigej.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gwgcryxlm.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gwwtaqvco.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gvbsszmkg.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gcokqoqyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gpxrlmria.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gzpkxrofp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gnaywffia.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gdpbgwsgm.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gopeujmxt.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gekoglaht.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gidexaofr.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gpkygpvqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gkyacctpg.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gatbgmler.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gvplxoerv.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gntkqwqvx.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gokjubvkh.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gehobjoce.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gymxvxoqp.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gmnmvhmpm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gtnrhpmhv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gdsjkevzg.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gkqtffohb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkpsffwve.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gndzzxxfi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtcmbbemv.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gxbpewiyd.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gauhiclvj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gcfctxpsa.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gabmekvlo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gekvniwaf.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gqcjwyvvz.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gjavkpaoj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gglsupqqi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gjtncclof.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqkobxu.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/grdfwabvm.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/giuedcqgg.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gvhkbjuug.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gakfncgpw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gawkthqph.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gcnbxpwhh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gryifacmn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gqigpupks.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gybtzgfpa.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/ghsnyzjir.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gpybibhyn.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gkbsxmdvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/ggqbkfmjf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/ghzfitdex.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gcivopwsc.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/ggzvflubk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gbhaowvsc.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gvpetyfhc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpuvpdshq.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/goxdvuond.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gexsbyyih.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gjrqxvphm.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gsoompxhz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gnfcszczh.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gxbcaghnf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gqlrckpff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gvkhfnxwr.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gbuqjyxaj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gzdlmondy.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/goemlgftr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbkfotlrr.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gochvrkrn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsgpoyixd.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gqrvarcwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gxlyxrmap.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gukqmuhgp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/geoqywyrd.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gjzrhrxmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gptsbekew.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gcujagrhe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gqugnvvqn.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/grlrxvqfk.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gxzurtuwe.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gfkhakubo.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gusvvecry.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/goixigdqt.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfpgkskzd.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gkovhjgge.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gvliyehze.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gqbwgdacf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gzorobwkm.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gqgtngafq.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gqmjgpfdi.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gkgrnwvsr.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gxnsdsfrp.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqvevenks.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gqxchrodr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gqctyvjdq.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/glwfcutnd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gxarevkdc.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gmbefdong.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gufqjrkos.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmzwtqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gnhvnnezr.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gtoaxtwrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcvzzbizt.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/guqtkcysc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gykfcdjgy.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gwicbeikk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/ghwgwokvg.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gaquqvvfv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gnxekgmnw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gkpphseur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/ggelugeag.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gyurhnexd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkmphtbo.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gaqeadrgz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gqlbcglfm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gmhhskmlu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gowskcziq.sHtML


<!-- 参考信息 -->