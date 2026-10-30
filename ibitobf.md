代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/glebwzapj.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gssrbjywm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gogpbxphb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/grrbxxiaw.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqeghtyn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/grazjqegx.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gmrbbbgro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gakisbxno.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxrkacick.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gqrfijsvg.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwtndcxi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gvluhqnyw.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gyskfbeol.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmrmorvf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnrbynen.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grborthbo.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gstievdsz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glfyxuixz.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gynpedyjt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcyrrlmx.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gxrpsqwfa.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjwgenbgh.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gskngnjhv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gvuvunjes.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxtrypnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcecoun.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhupxqgd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gqnwzzoba.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfxpwyvq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/grppgiprf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxvbfhxnu.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjswgnq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/goaxjewzu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxovosjeh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxbdpadl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpltjumcs.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeytbuaa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvqvybnwh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/goyclsvox.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbsezanb.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gqthvtqdd.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqmdelrm.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gbrtwdtqh.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/goqhrzoxc.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxjmguhw.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/glvmihide.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtolmxwoa.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gbqrqbcox.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkdtjfxr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gijoiczor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwopywcju.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gasrmqjum.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkpzftmo.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjwsbfkco.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/guluhjxes.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gqzzfhttc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gssppscia.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glurpugma.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqjzxkmtx.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/ghxvopoxt.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gxynnzcbv.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdnqjkv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrkmgezx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakvzwatj.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjwqhrgh.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkjxrlqb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzjjvaknx.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gqcqhuvvt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/guvcdkzwf.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvzeqwmh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwjhuzhms.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggukekiun.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyopmneim.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtbylxmwi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwoevrxi.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gcbpiuddn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfblmsvjh.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gjjszqhyu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqlrdwvdd.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrzpsorv.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gejsiiwoi.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfrgvujh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwvvvfvaf.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcvvnypli.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmguwldf.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gykrhlarq.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggcmcncen.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/giamzenhy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gavxtabvt.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqsoghzn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gftydogta.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdemjnytu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvtpklnn.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzygxyld.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjkmewbw.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlllrbvf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/giugytchn.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecskhmjn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytybnnbh.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/geyanohze.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbckeplfj.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpafioyvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtmmbhip.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grupfxihv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkvzsnyj.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gflooogrs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyeuzzopa.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gkzvowsgc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/galsqankf.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gzdiecdbe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsjjwvcnj.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gcbbdilix.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gotvhwrjm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyesyfgl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gdtewzkpy.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbktxauno.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybavnwqq.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoclruqd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrqxjdpr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gumlhvwhl.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdsiadaxe.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjwysmxo.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gsorbmpqj.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdnwtgjbi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseqtktxf.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqvdhyiu.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gapkbqaof.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giimusjse.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzbxnpof.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gjysnfldi.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gjyfvcgzd.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbhxjqmp.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/glmzgirxq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkfwzzfi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gazvbnpwl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgojstsz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbobgzqlf.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoecnytc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvuptgbru.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmxzbqft.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqgsnwyd.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggohbtkyi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggeknxmhx.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/glcpywtds.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzpyfpie.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwjkxmp.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdywjzsld.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gicxndrcl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzfmlxfih.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gasdikzjn.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjdldmwiy.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyngqjyr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfhdztgo.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gswgbkbbm.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gmycbwhcm.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gzboagmcw.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gpmujpsdl.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmiwrvnj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/guclprxyc.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgmxdmdq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkoqoagmp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gkrswbkmn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gppocwkxr.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gacjulwol.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuxuejop.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwcaigpi.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrhnnjke.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grtemyxcs.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/guwftyyhz.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/glyxzlgfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgdrmuem.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/grcmwcexk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnxeiwba.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gusnqiulv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssrdgvkd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/grnojasuv.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/grxineems.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/guunfreao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvikvkhoz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/giumacblq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgoaemtv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuehmoij.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guinxopkk.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gujsyotoa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqfonlji.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gyvilmafd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnpzvquh.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gltugezxw.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxuyfuf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwqiosmh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glbaalkct.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/girdaaffe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gzdbasjyk.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfjntdnrt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gtqsohpao.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gfppqevpu.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyiqfenv.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjeignh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuvdegwx.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gkkgpawiw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfgzdlhk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvylpbhb.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgqiidpc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdmbezkz.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvwhamlx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzohllij.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmrytsjbb.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmurriqhe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvijcjeod.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gopefwgxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gohukmlms.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/guftmjkof.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzdtabge.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjxmrlpz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpnqeeiy.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gndvgqpcu.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtqjwyon.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomtvwjha.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gwgsetwbl.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gntjrlcat.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmydqeksj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjkhvvey.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/guhujrbay.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkriobpfm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaiorgjf.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gxlfytbxm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gixjuzpua.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galhejezq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyivxcjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gecwmlazq.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grsvzwrrz.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/grrqkzier.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjxmdcmdz.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgkstml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmripsquj.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtkwaxwlf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxikgbzng.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/grkeftfna.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnpcxwhr.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gdjcqcfrs.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyvliuur.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtznlubfb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhxpdfpp.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gekcbixef.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/grxlsghag.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjmqgcuv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpiyxywb.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxingpto.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/guueohait.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gcihkirpo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkquvsdk.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/glbcbmxgv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplflimq.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcutqptk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/glqfwsgau.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gusrlbejr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganttlmgd.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gycnozeso.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwssvcdbx.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/glkgjridz.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcxlunhv.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvgwposr.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gporhfnfr.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrqigjdj.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gauhhpunv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcizcoyz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdnqqrzh.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gjchaastq.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/goxnycwcm.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccoacvib.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gdvghbvei.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxghcunc.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gcmustdfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gawazqgrh.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxezcdksx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gqjcebwmx.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gzbqdemsa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmzxjqezi.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwptqthx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxwumbrw.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzgyvyxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkgroctut.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gfmakwupv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhjegdtg.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/goquukdzr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gctiwkbmi.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guemmetee.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlavpqss.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gebtlnvfx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gttmevcab.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggbbdgbdc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gskpfgfsz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzejaqzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkmtwxakv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdswkgcb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gblqgrfit.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwypbyyge.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gganbyaif.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gckrxtrfz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeterrqm.sHtML


<!-- 参考信息 -->