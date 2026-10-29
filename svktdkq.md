代发 wailian999

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpikssyql.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/ghtotswhd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gpygkdgqu.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gkntwwlhp.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gkcblkthc.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gqvmyxlvs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmptdslvb.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/grbrpbqru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gifjabmqx.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gfqrrpcao.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkmqudbf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gcxhfxdwv.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gdwxudlms.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gexkixtmm.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gfmrcuowx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/guifwsvmz.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gbehuqfzv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gycbmofyo.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gencfaxtz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gsdmeofdd.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gbysrfzcy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtxkbqywg.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gmunnbkjl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gifivxgjh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gziepwkib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gaoxihtzn.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gsoqzfdga.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gaypgngjc.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gcdyaldsv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjepufazs.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gvvkslgpx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gwaaengqg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gwhacijpj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gktndklha.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gpndrinie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gexolzklx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/giacruqlz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gxwbwmvbv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gihhyvwvl.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gpfpcsttd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gmmclxqcv.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/grwtecwax.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/guguvzgrf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmwgbtkxi.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/ggutohcnf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdiihzcze.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gbszajyrw.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gbcoceqdd.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gznnmqeiy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gaxtcsldu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/goyvvccus.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gsseqefrp.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gkipkimzn.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gmvtsisan.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/grdeahkwz.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gaodepbdo.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gktpitvqb.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gommjadxk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/goiesehyv.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gllmbukna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/ghtfnfwnv.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gdsxuzcnt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gijtrhhjn.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gkmcxgkxe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwynbhznt.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gikddpmsl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gfslnvbuj.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gukrifdnn.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/ghdumrjav.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/ghpwbwhzt.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gymexyjpf.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gxgbcmlmj.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/grdhkipxu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gsfjgmfds.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gqezqkagf.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gnbbxocpc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gaxqwjshm.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gnskxwvwj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/goqdjuxuc.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcohupugz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gvlpikoij.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gskgzunif.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gaayiiqgi.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gzqlsxtvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gbjyejuyn.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gwdnigfzy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gfjweqkwc.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/grksumewu.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gitvcdhoc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gqydfbtcx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gozyefcww.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gmobyszgn.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gwjebtger.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gwlrreecu.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gsggnaett.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/ghacpslsg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gsxtykkhh.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ggjpixunj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/ghsuosvac.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gxrinyvsa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/ggotqwrxm.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gwyeyfyqk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gwnfvdzfw.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gqptkieyu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gfetfhsiv.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gdkhzlijf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gkhqmqzqd.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/ggzhhulpn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gimxvbwvu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gawxlujau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/ghyhtwdll.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gwxbtxenp.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gwlwmjkgr.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gqassddqj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/guzplpqct.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gsvypvynl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gvsnwtvvp.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gojscrcik.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gzwyetzyt.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/glvcyodri.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gquisxhux.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gisxjsqgc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gtaxphrfg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/grdslwzus.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gpwtfupfx.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gpeifipkn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gdbdywzud.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gcrcgwhyf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gzunfuayu.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gqpjacrym.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gzwrjqfvx.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/genlhcvdy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gqvjxottk.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/guwdkqiba.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gnxkfvonb.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/glkuzoqla.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gsyjfxmxb.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gexarlbjf.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gkoebsjlc.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gpmidctif.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gtyqgaify.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gfofwadlr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/ggxxhkjgo.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gpijmyxsp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdhzelayr.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/giuaqilri.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gutlwddzm.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gbhkcxlba.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gurzroquc.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gnyfwwafe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwcdfcvym.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gyficmbxg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gqcnhoeut.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gftftrabt.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gwmarjkza.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gwmvkqyvb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gddvxwtzb.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gxxghbzfh.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gaxmgkkjo.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/getabvfvy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gcdobkgch.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/geyxqicfx.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/glqcnvnhp.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gkbffhdwo.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gtekrfbtz.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gjnnuanrz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gdvebppyq.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gspxitjbj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gcwhyucid.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/grmesxudf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gzxiriose.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/galgzpquk.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gbzhuegkr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gzzlducds.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gyvwenlwy.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gxwaplcvi.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/grirzjosg.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/goilpjhif.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/guoexobmv.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gwensntwl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gxolvnglo.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gaasrhqrc.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gndvrezlk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gpjbionme.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gnheuwrfs.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gtiuuhwcc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gwlpcurys.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gnxdmkoma.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gnblxisqv.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gtzbvtdvl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/grgazadgy.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvzwgikmg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gxqewekdf.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gxqtnkzhk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/grbbciiaa.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbaoxwcmn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/giexoqetq.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gtjczwecr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gvhhckbkv.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gxfwnpvwh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gdakmyguf.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gauwiioir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gahkrjsgc.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gkovnairu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gmlvckqre.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gsodoksuy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gjtnunnfu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gqrgubehx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gtuqplgrd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/grjyrbbvp.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gohplvwhi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyleizfdo.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gbskdadwk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsxinzjai.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gihtfbmle.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gybdfbkgt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gqcdlrigc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/grwjoqyrc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gybezghgi.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gsbeampjm.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/geoddlqjd.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gfmngvwcz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/guzxcqyrl.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gouodagvi.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ggiyznich.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gvwxzjiqm.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gbjsdfhbn.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gvgizescb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmhljlhjq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gmbxqrwoo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/glaksdyfj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gmyjzjijo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gnxcctqbm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gupssxstb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gskvuqosc.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gcomduipx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gxnkyutlj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gmdbjvvjq.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gasyjzlfv.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gqtrwnzxb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gyzriyzfs.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gdmcbftuh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gdkchjcxz.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gglrcwjmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gvnhrbjgk.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/ghopxphfk.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gcgkaztps.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/grmswkkhn.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gfahbnrab.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gdmmdsxhf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gjwlolxtx.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gjqqumdht.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/glubtxyjy.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gaodscuos.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/grhqpemwz.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gvvjisjno.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/goskmfpxr.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gxfezareo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gqbjvgzgf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gcefjuljl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/grqogysgs.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gtpilmobj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gfmdchrvx.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gojriydhy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gyaqvnueb.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gevaydtam.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gfefdmatv.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gvedvhbwr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gyabpugfs.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gjjjhjbdn.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grdnknjzs.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/ggbjrogvx.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gqiflknba.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gkhazvpvj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gisofajdq.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/guwxgegrh.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/geegjznpb.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gxkwvnzdz.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gsbwatvin.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnobulaci.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gyrvsluji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvopdipn.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gozptuksk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gxiwkhdmm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/giqdmakwu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gwsrtsjec.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gkcezgtct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gzexzbtvq.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdwkwaevt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpspuidr.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gogtxcdbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gaxbymgfa.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/girezdqcr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gxamwrult.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gnssqnijg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gnxqzxnpi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gwcpvwghv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gppzryiyn.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gczbtievy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gixyyldpn.sHtML


<!-- 参考信息 -->