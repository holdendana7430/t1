代发 wailian999

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gpsmlfiqf.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gzdunclrp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gvccupyny.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gjmgrccze.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gbjfxfaub.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gfdvshzdb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gglehfzzh.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gzqjdrhrc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gkbstifku.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghfpharhg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzofjbdnc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gytvrvssp.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/giozcztor.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gbyoexffz.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gaofgzmyo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gfpjslgsy.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gyfhqlouc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gmfpjelzd.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gpefzxxev.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gvuesqsus.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gzofhrkdg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtqeqhnik.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gbdixazyo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvvaqzpvl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gqwaubtlu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdtnsakbp.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gmgdbyfjx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guewwqeak.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gjnwvxuax.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkbraumhq.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/ggwlrzyyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gqrbnxiok.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gvjesgsrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/glhqptnkx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gkitwkidm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gruzvgieb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gngdwjyqo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gklrjsgoi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvqnlfcmw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxxsoadfa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/giufuoawq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gyuxrrjqz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gxdfmqaau.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvkovgoxt.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gohlxtrln.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gilcnsphb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/goharqpwk.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gjsuescnr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/glcvccpan.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gnludraqf.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gbaaixhhm.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gexpfymcq.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gevllgjgs.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gpuclzthz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gsfyjujpd.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/goocayvbp.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gjxqhnxzs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfewzitlp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ggixxojlf.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gomwmetka.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjauoxsur.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gupnmpajc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/geuqthhcp.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/grbfvarny.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/geuoqbatg.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gkqtqtjqt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gbdfiybhl.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/grqueanea.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gjnkpyapu.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gfpbazoqv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqataggjp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gnbelulto.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gxyzxahly.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gqbwpawst.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gqdngvwwi.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/glwxbbgzj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gwmvjhqle.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gbdxuiszy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gupadkmee.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gytgmlsnb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gazassxpj.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gwfjauntc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gjbfoiyls.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gcbbugjst.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/ghaqbkhcd.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gprlmmrfr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gjhitliyf.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gmhcaeqav.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gwhluvlbj.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gmfonozpx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gyeaixazc.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gygylcnad.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gczsoupqm.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gftcgjyld.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gtdolahdy.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gvzajesnt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gjzbahuky.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gutfyqzqe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gndcekwap.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gfnrqexgi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/ggsjgslpl.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gnqiozrhy.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gumpyzzqu.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gyfuoqyqq.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gjizxklsg.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gortapxqm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/ghrqxgxit.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gnggamabr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gzkaysxac.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gkfpwnlda.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gcjxvgldj.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gefabrwdr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gufrysqim.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gdgfujpqa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gueppvfzi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gtwgbdhma.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/giiermacv.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/govwkyuyn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ggfdhcmch.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gyuxjabua.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gclalzeeu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gzyyxumaq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gzqzlyxwd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnxbryj.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gnhkxkctv.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gxzuzqlot.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gvnhcqfat.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/griyswusg.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghpctrddb.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gvuhukokx.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbwyxnpfs.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gnoasfrya.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwtcvsuvl.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gcrvbjuec.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gjxiomlen.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gcojjviag.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/ghfihdpfr.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/grwztonam.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gqdqgbosm.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gpicuowke.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gflgivlpq.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gcckpnymi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gwyqftftb.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gyovvmejh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghfwdpvjg.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gafwhbvjb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/giyrqdcbo.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gacxtftio.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gzxkybwbl.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/ginhcjkjt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/glmmyhzgl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gbnnywzai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gxthqamvl.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gfjmnurcf.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gyjrqbjoa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gsnxbsdkj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gcuqpcguq.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/giqvgxvil.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gvuumzymy.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gwtmodzit.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gphylenov.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gfeooctdk.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gxmccxyyf.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ghcqlqoqj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/ghwhwyutb.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gineiwxdc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gbzvpvrlc.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gkfsxbpla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gtodlptan.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gvimgkdwf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/guvpjrwom.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gtmrxznho.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gkxzupnes.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gzjxkyogg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gsjxhavec.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gczkjbykv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gtbxxefqk.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gjcppfylf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gtzductix.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gymwsrktu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gotijgmoz.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gjoallzxj.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gflayrcpx.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/guaeksfcc.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gshhqqdfe.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/glecmqbxw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gaicaevpu.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/guespyaif.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gubhefmbf.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gcjlfuhdg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gbbjlvkfn.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gbdjcmydd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gukcqgzbo.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gykppfgsu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gktfpoweo.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gjeiyakqj.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/ghgypsrsj.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gkxuyzntx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/grlsrdate.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gvhsdpgml.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/geowqcbyk.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gqwgscslw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/goiajxitn.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gkqeodxtx.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gctwoqlqa.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gsjfktzcd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gshhnayax.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ghkleadvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gagwjbdyz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gkwixvpqa.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/glusdycqu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggvpvsdyw.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gdcfxsgio.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmagagcoq.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/grpfvkxdt.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gbrosjmqe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gaimrsmuy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gievrsqje.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gfscgswdt.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gddottkbi.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gldklwvym.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gpcysfman.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gizeuwdip.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxokjeagq.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/glmpacdnw.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gvggoqwee.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gliwlvlav.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/ghklykoas.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gohdgurte.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gjbiemjnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gfllhdure.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/glsxenmnc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gejvilzde.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gdwcmgftk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gcyfabuig.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gqkvwiciw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gbddruibg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gumipmslx.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gfboawenj.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gtxxrhrfb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gpluniedz.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gtygbjude.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gwmwflieq.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gpbfhkblz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gwlekdjqp.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gzlmhntxq.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/geotivhpt.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gsoqrkqba.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gqhthytaf.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsxbjerao.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gzyxhfjuq.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gewkadluy.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gfhflmtjo.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gbegkvpaa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gbjitppnc.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gmhgxoqbs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gnrswmcgh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gudiafhyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/ghrhpvgfa.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gkqoqwwut.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gwpotoifx.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gqlhclahd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gnkurxhud.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gnnsccixm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gvxsjmshw.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gkyezrxxi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/geuoayrna.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gjdnaerei.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gpbkzfgmj.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gigltbarg.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gxrsfbbpo.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gxqpxoqto.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gqseeoryd.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gpgobpabq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gcdtdmggl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gqzfbljly.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gqeohplut.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/grbhcwegj.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gypoewhka.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/goixvzroz.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gudirxkma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gbxkmyyuf.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gorpurtyg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gnqphjyqn.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gznzwyhzm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/glojxgtph.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gdxjxubzg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gnjjzdndh.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gthuzwtnd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmbsdksqd.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/glskgxlpt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbxyqcuuf.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gytsxomwn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gyrcsowzb.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gqqgvbhwz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gwounozoo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/glrkrbags.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gnpwyvzgs.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gimxqlive.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gzglrfazt.sHtML


<!-- 参考信息 -->